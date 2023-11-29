<template>
    <div class=" formulario mt-5 " >
        <form>
            
            <input class="input1 form-control" type="text" placeholder="titulo de la tarea">
            <input class="input2 form-control" type="text" placeholder="Info de la tarea">
            <input class="input2 form-control" type="text" placeholder="Datos de la tarea">
            <input class="input2 form-control" type="date" >
            
        </form>
    </div>
</template>

<script setup lang="ts">

</script>

<style scoped>
.formulario{
    margin-left: 18%;
    
}
.input1{
    width: 550px;
    background-color: #d9d9d9;
}
@media (max-width: 1120px) {
  .formulario {
    margin-left: 10%;
    margin-top: 0%;

  }
}
@media (max-width: 670px) {
  .input1 {
    /* margin-left: 10%; */
    width: 300px;
    /* margin-top: 0%; */

  }
}
.input2{
    width: 1200px;
    margin-top: 12px;
    background-color: #d9d9d9;
}

@media (max-width: 1466px) {
  .input2 {
    /* margin-left: 10%; */
    width: 900px;
    /* margin-top: 0%; */

  }
}
@media (max-width: 1080px) {
  .input2 {
    /* margin-left: 10%; */
    width: 600px;
    /* margin-top: 0%; */

  }
}
@media (max-width: 670px) {
  .input2 {
    /* margin-left: 10%; */
    width: 300px;
    /* margin-top: 0%; */

  }
}
</style>