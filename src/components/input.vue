<template>
  <form @submit.prevent="submit">
  <input v-model="username" class="p-2 border border-color-grey" placeholder="username" type="text"/>
  <br>
  <input v-model="password" class="mt-2 p-2 border border-color-grey" placeholder="password" type="password"/>
    <br>
    <button type="submit" class="mt-2 bg-white p-2 border border-color-grey">Submit</button>
  </form>
</template>

<script>
  export default {
    name: 'inputForm',
    data(){
      return {
        username : "",
        password : "",
      }
    },
    methods:{
      submit(){
        console.log(this.username);
        console.log(this.password);
      }
    }
  }
</script>