<template>
  <div class="body">
    <div class="container">
      <div class="signin-signup">
        <div class="form-container" :class="{ 'form-left': !isSignInForm, 'form-right': isSignInForm }">
          <form v-if="isSignInForm" action="" class="sig-in-form">
            <h2 class="tittle">Sign in</h2>
            <div class="input-field">
              <i class="fas fa-user"></i>
              <input type="text" placeholder="Username">
            </div>
            <div class="input-field">
              <i class="fas fa-lock"></i>
              <input type="password" placeholder="password">
            </div>

            <button @click="toggleForm" type="button" class="btn btn-outline" id="sig-in-btn">Sign In</button>
          </form>
          <form v-else action="" class="sign-up-form">
            <h2 class="tittle">sign up</h2>
            <div class="input-field">
              <i class="fas fa-user"></i>
              <input class="color" type="text" placeholder="Username">
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

            <button @click="toggleForm" type="button" class="btn btn-outline" id="sig-up-btn">Sign Up</button>
          </form>
        </div>
        <div class="panel-container" :class="{ 'panel-left': !isSignInForm, 'panel-right': isSignInForm }">
          <div class="panel left-panel" v-if="isSignInForm">
            <!-- Contenido del panel izquierdo para Sign In -->
            <p class="color">El tiempo es más valioso que el <br> dinero, puedes conseguir más <br> dinero pero no puedes
              conseguir <br> más tiempo</p>
            <button @click="toggleForm" type="button" class="btn btn-outline" id="sig-in-btn">Sign In</button>
          </div>
          <div class="panel right-panel" v-else>
            <!-- Contenido del panel derecho para Sign Up -->
            <p class="color">Una buena vida se basa en <br> ser un buen gestor del <br> tiempo.</p>
            <button @click="toggleForm" type="button" class="btn btn-outline" id="sig-up-btn">Sign Up</button>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
   
<script lang="ts">
export default {
  data() {
    return {
      isSignInForm: true, // Iniciar con el formulario de inicio de sesión visible
    };
  },
  methods: {
    toggleForm() {
      this.isSignInForm = !this.isSignInForm;
    },
  },
};
</script>
   
<style scoped>
* {
  margin: 0;
  padding: 0;
  box-sizing: border-box;
  font-family: 'poppins', sans-serif;
  /* background-image: url(../assets/fondo.png);
     background-position: center;
     background-repeat: no-repeat;
     background-size: cover;
     background-attachment: fixed; */
}

.body {
  display: flex;
  justify-content: center;
  align-items: center;
  height: 100vh;
  background-image: url(../assets/fondo.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
}

.container {
  width: 60%;
  background-color: rgbas(120, 119, 123, 0.3);
}

.signin-signup {
  display: flex;
  justify-content: space-around;
  color: aliceblue;
}

.form-container {
  width: 50%;
  /* Ajusta el ancho del formulario según sea necesario */
}

.panel-container {
  width: 50%;
  /* Ajusta el ancho del panel según sea necesario */
}

.form-left {
  order: 1;
}

.form-right {
  order: 2;
}

.panel-right {
  order: 1;
}

.panel-left {
  order: 2;
}

input {
  background-color: #030A1C;
  color: white;
  border-radius: 0.5em;
  margin: 10px;
  text-align: center;

}

.color {
  color: white;
}
</style>