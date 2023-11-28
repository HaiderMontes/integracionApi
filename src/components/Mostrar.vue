<template>
  <div class="estilo">
    <div class="m-1">
      <h5>hacer ejercicio todas las mañanas antes de dormir</h5>
    </div>
    
    <div class="mar">
      <button class=" m-1 boton1 me-3">editar tarea</button>
      <button class= "m-1 boton2 ">eliminar tarea</button>
    </div>
  </div>
 
  
</template>

<style scoped>
.estilo {
  display: flex;
  justify-content: space-between; 
  background-color: #d9d9d9;
  color: black;
  margin-left: 14%;
  margin-right: 3%;
  margin-top: 20px;
  
  
}

@media (max-width: 1468px) {
  .estilo {
    margin-left: 16%;
    margin-right: 3%;
  }
}

@media (max-width: 1286px) {
  .estilo {
    margin-left: 20%;
    margin-right: 3%;
  }
}
@media (max-width: 1120px) {
  .estilo {
    margin-left: 2%;
    margin-right: 3%;
  }
}

@media (max-width: 442px) {
  .estilo {
    margin-left: 2%;
    margin-right: 2%;
  }
}

.mar {
  display: flex;
}
.boton1{
  background-color: #23d623;
  border-radius: 15px;
  width: 300px;
}
.boton2{
  background-color: #da0909;
  border-radius: 15px;
  width: 300px;
}
@media (max-width: 1176px) {
  .boton1 {
    width: 150px;
    height: 40px;
  }
}
@media (max-width: 1176px) {
  .boton2 {
    width: 150px;
    height: 40px;
  }
}

@media (max-width: 1328px) {
  .boton1 {
    width: 250px;
    height: 40px;
  }
}
@media (max-width: 1328px) {
  .boton2 {
    width: 250px;
    height: 40px;
  }
}
@media (max-width: 657px) {
  .boton1 {
    width: 100px;
    height: 60px;
  }
}
@media (max-width: 657px) {
  .boton2 {
    width: 100px;
    height: 60px;
  }
}


</style>
