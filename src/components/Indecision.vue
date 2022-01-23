<template>
  <img src="https://d500.epimg.net/cincodias/imagenes/2016/07/04/lifestyle/1467646262_522853_1467646344_noticia_normal.jpg"/>
  <div class="bg-dark"></div>
  <div class="indecision-container">
  <input placeholder="Introduzca su pregunta" type="text"/>
    <p>Recuerda termminar con un signo de interrogacion (?)</p>
    <div>
        <h2>Sere Millonario</h2>
        <h1>Si, no .... Pensando</h1>
    </div>
 </div>
</template>

<script>
export default {
    data(){
        return {
            counter: 10,
        }
    }
}
</script>

<style scoped>

    img, .bg-dark {
        height: 100vh;
        left: 0px;
        max-height: 100%;
        max-width: 100%;
        position: fixed;
        top: 0px;
        width: 100vw;
    }

    .bg-dark {
        background-color: rgba(0, 0, 0, 0.4);
    }

    .indecision-container {
        position: relative;
        z-index: 99;
    }
    
    input {
        width: 250px;
        padding: 10px 15px;
        border-radius: 5px;
        border: none;
    }
    input:focus {
        outline: none;
    }

    p {
        color: white;
        font-size: 20px;
        margin-top: 0px;
    }

    h1, h2 {
        color: white;
    }
    
    h2 {
        margin-top: 150px;
    }

</style>