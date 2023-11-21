<template>
  <div class="sidebar">
    <button class="burger-icon" @click="toggleMenu">&#9776;</button>
    <ul>
      <li><h6 class="titulo_app">MENU</h6></li>
      <li><a href="/">AGENDAR TAREA</a></li>
      <li><a href="/Tareas">MOSTRAR TAREAS</a></li>
      <li><a href="/login">CERRAR SECCION</a></li>
    </ul>
  </div>
</template>

<style>
.sidebar {
  margin: 4px;
  position: absolute;
  top: 0;
  left: 0;
  height: 100%;
  width: 200px;
  background-image: url(../assets/fondo.png);
  padding: 25px;
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
  margin-bottom: 10px;
}

a  {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
 
}
a:hover {
  font-family: 'Istok Web', sans-serif;
  color: blue;
  
}
.titulo_app  {
  color: #fff;
  text-decoration: none;
  cursor: pointer;
  text-align: center;
}


.table-container {
  display: none; /* Oculta la tabla por defecto */
  margin-top: 20px; /* Ajusta el margen para evitar la superposición con el menú */
}

@media (max-width: 1120px) {
  .sidebar {
    width: 100%;
    height: auto;
    position: relative;
  }

  .burger-icon {
    display: block; /* Mostrar el icono de hamburguesa en pantallas pequeñas */
    align-self: flex-end; /* Alinear el icono a la derecha en pantallas pequeñas */
  }

  ul {
    display: none; /* Ocultar la lista en pantallas pequeñas por defecto */
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