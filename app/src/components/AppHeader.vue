<template>
  <header class="header">
    oi
  </header>



  <!--
  <div :class="{'title':false, 'title-home': ishome}"> TITULO </div>
  <p class="['text', 'title]" > SDASDFSADFADISFJGIADUFIUSAFJIPUSDFJPIUSHFVSUHCPSIUHVNPSIUVHNSPIFUVBDIPVYBASPIVUCSDPVIUSVPIUSNVUIJ</p>
  
  <div class="todos" v-for="local in todos" v-bind:key="local.id">
    <img v-if="local.Vimg" v-bind:src="local.Vimg" v-bind:alt="local.imgAlt">

    {{ local.title }}
    
  </div>
  -->
  <div>
    <input v-model="name" type="text">
        {{name}}
  </div>
  <input
      v-model="colors"
      type="checkbox"
      value="Amarelo"
    />
    Amarelo <br>

    <input
      v-model="colors"
      type="checkbox"
      value="Azul"
    />
    Azul <br>

    <!-- Mostra os valores selecionados -->
    Selecionado: {{ colors }}
  


</template>

<script>
export default {
  name: 'AppHeader',  // vírgula aqui
  data() {
    return {

      name: 'joan snow',
      colors:[]
  


      /*pClass:"text",
      ishome: true,
      classVar:'title',
      todos: [
        {
          "userId": 1,
          "id": 1,
          "title": "delectus aut autem",
          "Vimg":'https://placehold.co/600x400',
          "imgAlt":"foto john snow",
          "completed": false
          
        },
        {
          "userId": 1,
          "id": 2,
          "title": "quis ut nam facilis et officia qui",
          "Vimg":'https://placehold.co/600x400',
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
      ]*/
    }
  }
}
</script>

<style>
.text{
  color:purple;
}
.title-home{
  color:green;
}
.title{
  color:red;
  font-size:200px;
  padding:1rem;
}
.header {
  background-color: #000;
  color: #fff;
}
</style>

<style>
.todos{
  background-color: #000;
  color: white;
}
.header {
  background-color: #000;
  color: #fff;
}
</style>
