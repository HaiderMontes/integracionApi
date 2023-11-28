<template>
    <div class="body">
        <div>
            <Navbar />
            <div class="titulo_tarea">
                <h1>MOSTRAR TAREAS</h1>
            </div>
            <Mostrar />

        </div>
    </div>
</template>

<script setup lang="ts">
import Navbar from '@/components/Navbar.vue';
import Mostrar from '@/components/Mostrar.vue';


</script>

<style scoped>
.titulo_tarea {
    text-align: center;
    background-image: url(../assets/fondo.png);
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    background-attachment: fixed;
    margin: 4px;
    color: white;
}

.body {
    width: 100%;
    height: 735px;

}
</style>