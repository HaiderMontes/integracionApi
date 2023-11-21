<template>
  <!-- <div class="container card-body"> -->
    <div class="table-responsive-sm container ">
      <table class="container table estilo color">
        <thead>
          <tr>

          </tr>
        </thead>
        <tbody>
          <tr>
            <div>
              <td scope="col ">
                  *hacer ejerccio
              </td>
            </div>
            <div>
              <td scope="col">
                <button class="boton btn btn-success me-3">editar tarea</button>
                <button class="boton btn btn-danger">eliminar tarea</button>
              </td>
            </div>
          </tr>
          <tr class="">
            <div>
              <td scope="col">
                <div>
                  *hacer ejerccios en la mañana antes de ir al trabajo
                </div>
              </td>
            </div>
            <div>
              <td scope="col">
                <button class="boton btn btn-success me-3">editar tarea</button>
                <button class="boton btn btn-danger">eliminar tarea</button>
              </td>
            </div>
          </tr>
        </tbody>
      </table>
    </div>

  <!-- </div> -->

  
</template>

<script lang="ts">

</script>

<style scoped>
@media (max-width: 992px) {
  .boton {
    width: 100%;
    height: auto;
    position: relative;
    margin-top: 4px;
  }
}
@media (max-width: 1120px) {
  .estilo {
    margin-left: 0%;
    width: 85%;
    margin-left: 8%;
  }
}

.estilo{
 
  max-width: 45em;
  background-color: #b3e5fc;
  margin-top: 50px;
}
</style>

