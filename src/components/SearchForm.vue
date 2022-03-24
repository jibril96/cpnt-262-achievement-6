<template>
    <div>
       <input type="text" placeholder="Search" v-model="name" />  
    </div>
    <div>
        <button v-on:click="submitForm">Search</button>
    </div>
</template>
<script>
import{ref} from 'vue'
export default {
    setup() {

        const name = ref('')

        const submitForm = () => {
            console.log(`Search submitted! Name = ${name.value}`)

        }

        return {
            name,
            submitForm,
        }
        
    },
}
</script>


<style>
input[type='text'] {

    padding: 5px;
    width: 400px;
    background: lightgray;

}

button {

 background-color: #fbff0046; 
  border: none;
  color: rgb(0, 255, 13);
  padding: 15px 32px;
  text-align: center;
  align-items: center;
  font-size: 16px;
    margin: 20px;
    width: 100px;
    border-radius: 8px;
    cursor: pointer;

}

button:hover {

  background-color: #af4c4c; 
  color: white;
}
</style>