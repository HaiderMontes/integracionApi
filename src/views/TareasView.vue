<template>
    <div class="body">
        <div>
            <Navbar />
            <div class="titulo_tarea">
                <h1>MOSTRAR TAREAS</h1>
            </div>
            <Tabla />

        </div>
    </div>
</template>

<script setup lang="ts">
import Navbar from '@/components/Navbar.vue';
import Tabla from '@/components/Tabla.vue';


</script>

<style scoped>
.titulo_tarea {
    text-align: center;
    background-image: url(../assets/fondo.png);
    margin: 4px;
    color: white;
}
.body{
    width: 100%;
    height: 800px;
    background-color: #9fa8da;
}
</style>