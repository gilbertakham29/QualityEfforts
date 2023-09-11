<template>
    <div>
        <h1 class="text-3xl text-center font-semibold mb-4">Todo List App</h1>
        <div class="mb-6 mt-6 flex flex-col justify-between items-center">
            <input v-model="newTodo" class="w-1/2 rounded-lg border-gray-700 border-solid  p-2" placeholder="Add a new Todo here...">
            <button @click="addTodo" class="bg-blue-500 text0-white px-10 py-2 rounded-lg my-5">Add</button>
        </div>
        <div v-for="(todo,index) in todoList" :key="index" class=" w-1/2 flex bg-[#FEF9EC] justify-between items-center mb-4 mx-auto">
        <span>{{ todo }}</span>
        <button @click="deletTodo(index)" class="bg-red-500 text0-white px-4 py-2 rounded-lg">Remove</button>
    </div>
    </div>
</template>

<script>
export default{
    data(){
        return {
            newTodo:"",
            todoList:[]
        }
    },
    methods:{
        addTodo(){
            if(this.newTodo){
                this.todoList.push(this.newTodo)
                this.newTodo = ""
            }
        },
        deletTodo(index){
            this.todoList.splice(index,1)
        }
    }
}
</script>

<style scoped>

</style>