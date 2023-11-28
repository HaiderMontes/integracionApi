<template>
     <div class="body">
          <div class="container">
               <div class="signin-signup">
                    <form action="" class="sig-in-form">
                         <h2 class="tittle">sign in</h2>
                         <div class="input-field">
                              <i class="fas fa-user"></i>
                              <input type="text" placeholder="Username">
                         </div>
                         <div class="input-field">
                              <i class="fas fa-lock"></i>
                              <input type="password" placeholder="password">
                         </div>
                         <button type="button" class="btn btn-outline">Enter</button>
                         
                    </form>
                    <form action="" class="sign-up-form">
                         <h2 class="tittle">sign</h2>
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
                         <button type="button" class="btn btn-outline">Enter</button>
                    </form>
               </div>
               <div class="panels-container">
                    <div class="panel left-panel">
                         <div class="content">
                              <p>El tiempo es mas valioso que el dinero, puedes conseguir mas dinero pero no puedes conseguir
                                   mas tiempo</p>
                              <button type="button" class="btn btn-outline" id="sig-in-btn">sig in</button>
                         </div>

                    </div>
                    <div class="panel right-panel">
                         <div class="content">
                              <p>Una buena vida se basa en ser un buen gestor del tiempo.</p>
                              <button type="button" class="btn btn-outline" id="sig-up-btn">sign up</button>
                         </div>
                    </div>
               </div>
          </div>
     </div>
</template>

<script lang="ts">
 const sig_in_btn = document.querySelector("sign-in-btn");
 const sig_up_btn = document.querySelector("sign-up-btn");
 const container = document.querySelector(".container");

 sig_up_btn?.addEventListener("click", () => {
     container?.classList.add("sig-up-mode");
 });

 sig_in_btn?.addEventListener("click", () => {
     container?.classList.remove("sig-in-mode");
 });


</script>

<style scoped>
* {
     margin: 0;
     padding: 0;
     box-sizing: border-box;
     font-family: 'poppins', sans-serif;
     background-image: url(../assets/fondo.png);
     background-position: center;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed;
}

.body {
     display: flex;
     align-items: center;
     justify-content: center;
     min-height: 100vh;
     
     /*  background-image: url(../assets/fondo.png);
     background-position: center;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed; */
}

.container {
     position: relative;
     width: 70vw;
     height: 80vh;
     /* background-image: url(../assets/fondo.png); */
     box-shadow: 0 4px 20px 0 rgba(0, 0, 0, 0.3), 0 6px 20px 0 rgba(0, 0, 0, 0.3);
     overflow: hidden;
     /*
      background-position: center;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed; */

}

.container::before {
     content: "";
     position: absolute;
     top: 0;
     left: -50%;
     width: 100%;
     height: 100%;
     /* background-image: url(../assets/fondo.png); */
     z-index: 6;
     transform: translateX(100%);
     transition: 1s ease-in-out;
     /* background-position: center;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed;  */

}

.sigin-sigup{
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     display: flex;
     align-items: center;
     justify-content: space-around;
     z-index: 5;
}

form {
     display: flex;
     align-items: center;
     justify-content: center;
     flex-direction: column;
     width: 40%;
     min-width: 238px;
     padding: 0 10px;
}

form.sig-in-form{
     opacity: 1;
     transition: 0.5s ease-in-out;
     -o-transition-delay: 1s;
}

form.sig-up-form{
     opacity: 0;
     transition: 0.5s ease-in-out;
     -o-transition-delay: 1s;
}

.tittle {
     font-size: 35px;
     color: #fff;
     margin-bottom: 20px;
}

.input-field {
     width: 100%;
     height: 50%;
     margin: 10px 0;
     border: 2px solid rgb(1, 1, 34);
     border-radius: 50px;
     display: flex;
     align-items: center;
     background-color: rgb(1, 1, 34);
}

.input-field i {
     flex: 1;
     text-align: center;
     color: #666;
     font-size: 18px;
}

.input-field input {
     flex: 5;
     background: none;
     border: none;
     outline: none;
     width: 100%;
     font-size: 18px;
     font-weight: 600;
     color: #7c7a7a;
}

.btn {
     width: 100px;
     height: 30px;
     /* border: none; */
     border-radius: 50px;
     background-color: rgb(1, 1, 34);
     color: #666;
     font-weight: 600;
     margin: 10px 0;
     text-transform: uppercase;
     cursor: pointer;
}

.btn:hover{
     background: #666;
}
.panels-container {
     position: absolute;
     top: 0;
     left: 0;
     width: 100%;
     height: 100%;
     display: flex;
     align-items: center;
     justify-content: space-around;
}

.panel {
     display: flex;
     flex-direction: column;
     align-items: center;
     justify-content: space-around;
     width: 35%;
     min-width: 238px;
     padding: 0 10px;
     text-align: center;
     z-index: 6;
}

.left-panel{
     pointer-events: none;
}
.content {
     color: #fff;
     transition: 1.1s ease-in-out;
     transition-delay: 0.5s;
}

.panel p {
     font-size: 15px;
     padding: 10px 0;

}

.left-panel.image,
.left-panel.content {
     transform: translateX(-200%);
}

.right-panel.image,
.right-panel.content {
     transform: translateX(0);
}


.container.sig-up-mode::before {
     transform: translateX(0);
}


.container.sig-up-mode.right-panel.image,

.container.sig-up-mode.right-panel.content, {
     transform:translateX(200%) ;
}

.container.sig-up-mode.left-panel.image,

.container.sig-up-mode.left-panel.content,{
     transform:translateX(0) ;
}

.container.container.sig-in-mode.form.sig-in-form{
     opacity: 0;
}

.container.container.sig-up-mode.form.sig-in-form{
     opacity: 0;
}
.container.sig-up-mode.right-panel{
     pointer-events: none;
}

.container.sig-up-mode.left-panel{
     pointer-events: all;
}

/*responsive*/

@media(max-width:779px){
     .container{
          width: 100vw;
          height: 100vh;
     }
}

@media(max-width:635px){
     .container::before{
          display: none;
     }
     form{
          width: 80%;
     }
     .form.sig-up-form{
          display: none;
     }
     .panels-container{
          display: none;
     }
}

</style>