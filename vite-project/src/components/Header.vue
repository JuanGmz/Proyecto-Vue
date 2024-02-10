<script setup>

</script>

<template>

    <div class="contenido">
        <h4 class="logo">Juan Gómez</h4>
        
        <div class="contenedor">
            <a href="#">Inicio</a>
            <a href="#">Sobre Mí</a>
            <a href="#">Contactame</a>
        </div>
    </div>
    
</template>

<style>
    .contenido {
        display: grid;
        grid-template-columns: auto auto;
        grid-template-rows: auto auto auto;
        align-items: center;
    }
    .contenedor {
        display: flex;
        justify-content: space-evenly;
        margin: 40px;
    }
    .contenedor a {
        font-size: 700;
        font-weight: bold;
        color: #FFF;
        text-decoration: none;
    }
    .logo {
        grid-row: 1;
        text-align: center;
        color: #FFF;
    }
    @media (max-width: 768px) {
        .contenido {
            display: grid;
            grid-template-columns: auto;
            grid-template-rows: auto auto;
            align-items: center;
        }
        .contenedor {
            display: flex;
            flex-direction: column;
            gap: 30px;
            text-align: center;
        }
        .logo {
            grid-row: 1;
            grid-column: 1;
            text-align: center;
        }
    }
</style>