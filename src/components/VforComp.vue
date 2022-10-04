<template>
    <my-component
  v-for="(item, index) in items"
  v-bind:item="item"
  v-bind:index="index"
  v-bind:key="item.id"
></my-component>

    <div id="todo-list-example">
        <form v-on:submit.prevent="addNewTodo">
            <label for="new-todo">Agreg Fruta:</label>
            <br/>
            
            <br/>
            <input v-model="newTodoText" 
            id="new-todo" placeholder="Fruta">
            
            <button>Añadir</button>
        </form>
        <ul>
            <li 
            v-for="(todo,index) in todos"
            v-bind:key="todo.id"
            v-bind:title="todo.title"
            v-on:remove="todos.splice(index,1)"
            this="todo-item">{{todo.title}}
                
            </li>
        </ul>
        
    </div>

</template>
<script>




    export default{
        data(){
            return{
                newTodoText: '',
                todos:[
                    {id:1,title:'take'},
                    

            ],
            nextTodoId:2
            }
            
        },
        methods:{
            addNewTodo:function(){
                this.todos.push({
                    id: this.nextTodoId++,
                    title:this.newTodoText
                })
                this.newTodoText=''
            }
        }
    }
</script>
    
 