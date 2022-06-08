<template>
  <div class="p-2 mt-5">
    <h1>{{ msg }}</h1>
    <inputForm />
  </div>
</template>

<script>
import inputForm from './input'

export default {
  name: 'UserForm',
  components: {
    inputForm
  },
  props: {
    msg: String
  }
}
</script>
