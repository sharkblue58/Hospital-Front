<template>
  <link href='https://unpkg.com/boxicons@2.1.4/css/boxicons.min.css' rel='stylesheet'>
  <section class="container forms">
      <div class="form login">
        <div class="form-content">
          <header>Sign Up</header>
          <form action="#">
            <div class="field input-field">
              <input type="first name" placeholder="first name" class="input">
             </div>

             <div class="field input-field">
              <input type="last name" placeholder="last name" class="input">
             </div>

             <div class="field input-field">
              <input type="phone" placeholder="phone" class="input">
             </div>
  
             <div class="field input-field">
              <input type="email" placeholder="email" class="input">
             </div>
  
             <div class="field input-field">
              <input type="password" placeholder="password" class="password">
              <i class='bx bx-hide eye-icon'></i>
             </div>

             <div class="field input-field">
              <input type="password" placeholder="confirm password" class="password">
              <i class='bx bx-hide eye-icon'></i>
             </div>
            
  
             <div class="field button-field">
              <button>Register</button>
             </div>
  
          </form>
          <div class="form-link">
                <span>Contact us?<a href="#" class="signup-up">visit</a></span>
              </div> 
        </div>
      </div>
  </section>
  </template>
<script>
export default{
    name : 'SignUp'
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

</style>