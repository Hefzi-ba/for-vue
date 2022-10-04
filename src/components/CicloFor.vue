<template>
    <div>
        <ol>
            <li v-for="(item,index) in array" :key="index">{{index}},{{ item }}</li>
        </ol>
    </div>
</template>
<script>
    export default{
        data(){
            return{
                array:["php","C#","JavaScript","python","java"]
            }
        }
    }
</script>