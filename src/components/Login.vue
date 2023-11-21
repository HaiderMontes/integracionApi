<template>
     <div class="body">
    <div class="container">
      <div class="login-register">
      <form action="" class="log-in-form">
      <h2 class="tittle">lOGIN</h2>
      <div class="input-field">
           <i class="fas fa-user"></i>
           <input type="text" placeholder="Username">
      </div>
      <div class="input-field">
           <i class="fas fa-lock"></i>
           <input type="password" placeholder="password">
      </div>
      <input type="submit" value="ENTER" class="btn">
       </form>
       <form action="" class="REGISTER-up-form">
      <h2 class="tittle">REGISTER</h2>
      <div class="input-field">
           <i class="fas fa-user"></i>
           <input type="text" placeholder="Username">
      </div>
      <div class="input-field">
           <i class="fas fa-lock"></i>
           <input type="password" placeholder="password">
      </div>
      <div class="input-field">
           <i class="fas fa-envelope"></i>
           <input type="text" placeholder="name">
      </div>
      <div class="input-field">
           <i class="fas fa-envelope"></i>
           <input type="text" placeholder="Email">
      </div>
      <input type="submit" value="ENTER" class="btn">
       </form>
    </div>
    <div class="panels-container"></div>
    </div>
</div>
</template>

<script lang="ts">

</script>

<style scoped>
*{
     margin: 0;
     padding: 0;
     box-sizing: border-box;
     font-family: 'poppins', sans-serif;
     
}
.body{
  display: flex;
  align-items: center;
  justify-content: center;
  min-height: 100vh;
  background-image: url(../assets/fondo.png);
}
.container{
     position: relative;
     width: 70vw;
     height: 80vh;
     background-image: url(../assets/fondo.png);
     box-shadow: 0 4px 20px 0 rgba(0, 0, 0, 0.3), 0 6px 20px 0 rgba(0, 0, 0, 0.3);
}
.login-register{
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     display: flex;
     align-items: center;
     justify-content: space-around;
}
form{
     display: flex;
     align-items: center;
     justify-content: center;
     flex-direction: column;
     width: 40%;
     min-width: 238px;
     padding: 0 10px;
}
.tittle{
     font-size: 35px;
     color: #fff;
     margin-bottom: 20px;
}
.input-field{
     width:100%;
     height: 50%;
     margin: 10px 0;
     border:2px solid #000;
     border-radius: 50px;
     display: flex;
     align-items: center;
}
.input-field i{
     flex: 1;
     text-align: center;
     color: #666;
     font-size: 18px;
}
.input-field input{
     flex: 5;

}

</style>