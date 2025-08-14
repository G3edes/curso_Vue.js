<template>
  <header class="header">
    oi
  </header>
  <div v-for="local in todos" :key="local.id">
    {{ local.title }}
  </div>
</template>

<script>
export default {
  name: 'AppHeader',  // vírgula aqui
  data() {
    return {
      todos: [
        {
          "userId": 1,
          "id": 1,
          "title": "delectus aut autem",
          "completed": false
        },
        {
          "userId": 1,
          "id": 2,
          "title": "quis ut nam facilis et officia qui",
          "completed": false
        },
        {
          "userId": 1,
          "id": 3,
          "title": "fugiat veniam minus",
          "completed": false
        },
        {
          "userId": 1,
          "id": 4,
          "title": "et porro tempora",
          "completed": true
        }
      ]
    }
  }
}
</script>

<style>
.header {
  background-color: #000;
  color: #fff;
}
</style>

<style>
.header {
  background-color: #000;
  color: #fff;
}
</style>
