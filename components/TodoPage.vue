<template>
    <div>
        <h1 class="text-3xl text-center font-semibold mb-4">Todo List App</h1>
        <div class="mb-6 mt-6 flex flex-col justify-between items-center">
            <input v-model="newTodo" v-on:keyup.enter="addTodo" class="w-1/2 rounded-lg border border-gray-700 border-solid  p-2" placeholder="Add a new Todo here...">
            <button @click="addTodo" class="bg-blue-500 text0-white px-10 py-2 rounded-lg my-5">Add</button>
        </div>
        <div v-for="(todo,index) in todoList" :key="index" class=" w-1/2 flex bg-[#FEF9EC] justify-between items-center mb-4 mx-auto">
            <div v-if="index === editedIndex" class="flex justify-between items-center flex-row w-full">
            <input v-model="editedTodo" @keyup.enter="updatedTodo" @keyup.esc="cancelEdit" class="w-1/2 rounded-lg border border-gray-700 border-solid  p-2">
            <button type="button" @click="updatedTodo" class="text-gray-900 bg-white border border-gray-300 focus:outline-none hover:bg-gray-100 focus:ring-4 focus:ring-gray-200 font-medium rounded-lg text-sm px-5 py-2.5 mr-2 dark:bg-gray-800 dark:text-white dark:border-gray-600 dark:hover:bg-gray-700 dark:hover:border-gray-600 dark:focus:ring-gray-700">Save</button>
            </div>
            <div class="flex justify-between items-end flex-row w-full" v-else>
                <span class="text-2xl font-semibold font-mono">{{ todo }}</span>
                <div class="flex justify-between items-center flex-row">
            <button @click="startEdit(index)" class="bg-green-300 text-white px-8 mx-1 py-2 rounded-lg">Edit</button>
        <button @click="deletTodo(index)" class="bg-red-500 text-white px-4 py-2 rounded-lg">Remove</button>
        </div>
            </div>
       
    </div>
    </div>
</template>

<script>
export default{
    data(){
        return {
            newTodo:"",
            todoList:[],
            editedIndex:-1,
            editedTodo:""
        }
    },
    methods:{
        addTodo(){
            if(this.newTodo){
                this.todoList.push(this.newTodo)
                this.newTodo = ""
            }
        },
       startEdit(index){
        this.editedIndex = index
        this.editedTodo = this.todoList[index];
       },
       updatedTodo(){
        if(this.editedTodo){
            this.todoList[this.editedIndex] = this.editedTodo
            this.cancelEdit()
        }
       },
       cancelEdit(){
        this.editedIndex = -1
        this.editedTodo = ""
       },
        deletTodo(index){
            this.todoList.splice(index,1)
        }
    }
}
</script>

<style scoped>

</style>