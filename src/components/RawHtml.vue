<template>
    <div>
       <p> {{rawhtml}}</p>
       <hr>
       <p v-html="rawhtml"></p>
    </div>
</template>
<script>
    export default{
        data(){
            return{
            rawhtml:'<span class="colorRojo">Hola Texto Rojo</span>'
            }
        }
    }
</script>
<style>
    .colorRojo{
        color:red;
    }
</style>