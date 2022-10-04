<template>
    <div>
        <input v-model="message" placeholder="edíteme">
        <p>El mensaje es: {{ message }}</p>
        <button value="submit">hi</button>
        <hr>
        <ul>
            <li v-for="message in Array" :key="message">{{ message }}</li>
        </ul>
        
    </div>
</template>
<script>


    
        
        export default{
            data(){
                return{
                    message:{message:''},
                    Array:["message:''"]
                }
            }
        }
        
    
</script>