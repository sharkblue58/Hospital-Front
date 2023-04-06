<template>
<link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
<section class="container forms">
    <div class="form login">
      <div class="form-content">
        <header>Sign In</header>
        <form action="#">

           <div class="field input-field">
            <input type="email" placeholder="email" class="input">
           </div>

           <div class="field input-field">
            <input type="password" placeholder="password" class="password">
            <i class='bx bx-hide eye-icon'></i>
           </div>
          
            <div class="form-link">
              <a href="#" class="forgot-pass">Forget password</a>
            </div>   

           <div class="field button-field">
            <button>Login</button>
           </div>

        </form>
        <div class="form-link">
              <span>Already have an account?<a href="./SignUp.vue" class="signup-up">Signup</a></span>
            </div> 
      </div>
      <div class="line"></div>
      <div class="media-options">
          <a href="#" class="field facebook">
              <i class='bx bxl-facebook facebook-icon'></i>
              <span>Login with Facebook</span>
          </a>
      </div>
      <div class="media-options">
          <a href="#" class="field google">
              <img src="../assets/google.png" alt="" class="google-img">
              <span>Login with Google</span>
          </a>
      </div>
    </div>

</section>
</template>
<script>
export default{
    name : 'SignIn'
}
</script>
<style>
@import url('https://fonts.googleapis.com/css2?family=Poppins:ital,wght@0,300;0,400;0,500;1,600&display=swap');
*{
    margin: 0;
    padding: 0;
    box-sizing: border-box;
    font-family: 'Poppins', sans-serif;
}
.container{
  height: 100vh;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
  background-color: #4070f4;
}
.form{
  max-width:430px;
  width: 100%;
  padding: 30px;
  border-radius: 6px;
  background: #fff;
}
header{
  font-size: 28px;
  font-weight: 600;
  color:#232836 ;
  text-align:center;
}
form{
  margin-top:30px;
}
.form .field{
  position: relative;
  height: 50px;
  width: 100%;
  margin-top: 20px;
  border-radius: 6px;
}
.field input,
.field button{
  height: 100%;
  width: 100%;
  font-size: 16px;
  font-weight: 400;
  border: none;
  border-radius: 6px;
}
.field input{
 
  padding: 0 15px;
  border: 1px solid #CACACA;
  outline: none;
}
.field input:focus{
border-bottom-width: 2px;
}
.eye-icon{
  position: absolute;
  top: 50%;
  right: 10px;
  transform: translateY(-50%);
  cursor: pointer;
  padding: 5px;
  font-size: 18px;
  color: #8b8b8b;
}
.field button{
  color: #fff;
  background-color: #0171d3;
  transition: all 0.3s ease;
  cursor: pointer;
}
.field button:hover{
  
  background-color: #016dcb;
}
.form-link{
  text-align: center;
  margin-top: 10px;
}
.form-link span,
.form-link  a
{
 font-size: 14px;
 font-weight: 400;
 color: #232836;
}
.form a {
  color: #0171d3;
  text-decoration: none;
}
.form-content a:hover {
  text-decoration: underline;
}
.line{
  position: relative;
  height: 1px;
  width: 100%;
  background-color: #d4d4d4;
  margin: 36px 0;
}
.line::before{
  content: 'or';
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%,-50%);
  background-color: #fff;
  color: #232836;
  padding: 0 15px;
}
.media-options a{
display: flex;
background-color: #fff;
align-items: center;
justify-content: center;
}
a.facebook{
  color: #fff;
  background-color: #4267b2;
}
a.facebook .facebook-icon{
height: 28px;
width: 28px;
color: #0171d3;
font-size: 20px;
border-radius: 50%;
display: flex;
align-items: center;
justify-content: center;
background-color: #fff;
}
.facebook-icon,
img.google-img{
  position: absolute;
  top:50%;
  left:15px;
  transform: translateY(-50%);
}
img.google-img{
  height: 23px;
  width: 23px;
  object-fit: cover;
}
a.google{
  border: 1px solid #CACACA;
}
a.google span{
  font-weight: 500;
  opacity: 0.6;
  color: #232836;
}
</style>