<template>
    <div id="app">
        <h1>Конвертер</h1>
        <div class="line">
            <Converter currA="USD" currB="BRL"></Converter>
            <Converter currA="BRL" currB="USD"></Converter>
        </div>
        <div class="line">
            <Converter currA="CAD" currB="BRL"></Converter>
            <Converter currA="BRL" currB="CAD"></Converter>
        </div>
        <div class="line">
            <Converter currA="EUR" currB="BRL"></Converter>
            <Converter currA="BRL" currB="EUR"></Converter>
        </div>
    </div>
</template>



<script>

    import Converter from "./components/Converter.vue";

    export default {
        name: 'app',
        components: {
            Converter
        }
    };
</script>

<style>
     body{
       background-image: url("18Pe.gif");
     }

    #app {
        max-width: 900px;
        margin: auto;
        font-family: 'Avenir', Helvetica, Arial, sans-serif;
        -webkit-font-smoothing: antialiased;
        -moz-osx-font-smoothing: grayscale;
        text-align: center;
        color: #DC143C;
        margin-top: 60px;


    }

    .line {
        margin-top: 40px;
        display: flex;
        justify-content: space-around;
    }

    .footerStyle {
        margin-top: 20px;
        text-align: right;
        font-size: 9px;
    }


</style>