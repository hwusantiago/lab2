<template>
   <div id="login-box">
      <div class="left">
         <h1>Sign up</h1>
         <form action="/signup" method="post">
               <input type="text" v-model="userData.username" placeholder="Username" />
               <input type="text" v-model="userData.email" placeholder="E-mail" />
               <input type="password" v-model="userData.password" placeholder="Password" />
               <input type="password" name="password2" placeholder="Retype password" />
               <input type="submit" name="signup_submit" value="Sign me up" />
         </form>
      </div>
   
      <div class="right">
         <span class="loginwith">Sign in with<br />social network</span>
         <button class="social-signin facebook">Log in with facebook</button>
         <button class="social-signin twitter">Log in with Twitter</button>
         <button class="social-signin google">Log in with Google+</button>
      </div>
      <div class="or">OR</div>
   </div>
  </template>
  
  <script>
 export default {
    name: 'signupPage',
    data() {
      return {
         userData : {
            username: '',
            email: '',
            password: ''
         }
      }
    }
 }
  </script>
  
  <style scoped>
 
  </style>