<template>
  <div class="sidebar">
    <button class="burger-icon" @click="toggleMenu">&#9776;</button>
    <ul>
      <li><h6 class="mb-3 titulo_app">MENU</h6></li>
      <li class="bor"><a href="/formulario">AGENDAR TAREA</a></li>
      <li class="bor"><a href="/Tareas">MOSTRAR TAREAS</a></li>
      <li class="bor"><a href="/">CERRAR SECCION</a></li>
    </ul>
  </div>
</template>

<style>
.sidebar {
  margin-top: 4px;
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 200px;
  background-image: url(../assets/fondo.png);
  background-position: center;
  background-repeat: no-repeat;
  background-size: cover;
  background-attachment: fixed;
  box-sizing: border-box;
  display: flex;
  flex-direction: column;
}

.burger-icon {
  display: none; 
  font-size: 24px;
  background-color: transparent;
  color: #fff;
  border: none;
  cursor: pointer;
}

ul {
  list-style: none;
  margin: 12PX;
  padding: 0;
}

li {
  /* margin-bottom: 10px; */
  border-bottom: 1px solid #fff; 
  padding-bottom: 0px;
  padding-top: 0px;
  border-bottom: 1px solid #fff;
}
.bor {
  /* margin-bottom: 10px; */
  border-bottom: 1px solid #fff; 
  padding-bottom: 10px;
  padding-top: 10px;
  border-bottom: 1px solid #fff;
}

a  {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
 
}
a:hover{
  color: aqua;
}
.titulo_app  {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
  text-align: center;
}


.table-container {
  display: none; 
  margin-top: 20px; 
}

@media (max-width: 1120px) {
  .sidebar {
    width: 100%;
    height: auto;
    position: relative;
  }

  .burger-icon {
    display: block;
    align-self: flex-end; 
  }

  ul {
    display: none; 
  }

  ul.show {
    display: flex;
    flex-direction: column;
  }

  
}
</style>

<script>
export default {
  data() {
    return {
      showContactTable: false
    };
  },
  methods: {
    toggleMenu() {
      const menu = document.querySelector('.sidebar ul');
      menu.classList.toggle('show');
    },
    showTable() {
      this.showContactTable = true;
    }
  }
}
</script>