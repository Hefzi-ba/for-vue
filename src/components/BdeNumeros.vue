<template>
    <div >
        <button v-on:click="con += 1">Add 1</button>
        <p>Se ha hecho clic en el botón de arriba {{ con }} veces.</p>

        <hr>

        <input v-model="fruta" placeholder="fruta">
        <button v-on:click="array=fruta">Añadir</button>
        <p>Se ha añadio:{{ array }} </p>
        <ol>
            <li v-for="fruta in array" :key="fruta">{{fruta}}</li>
        </ol>
        
    </div>
</template>
<script>
    
     export default{
        data(){
            return{
                con:0,
                array:{fruta:''}
            }
           
        }
     }
</script>