<template>
<v-layout>
<v-card 
class="mx-auto"
max-width="200"
v-for="(personaje,index) in this.personajes" :key="index"> 
<v-img class="white--text align-end" height="200px" :src="personaje.imagen">
</v-img>
<v-card-subtitle>{{personaje.nombre}}</v-card-subtitle>
</v-card>
</v-layout>
</template>

<script>
export default {
    data(){ 
        return{
                  personajes: [
        {
          id: 1,
          nombre: "Morty",
          imagen: "https://rickandmortyapi.com/api/character/avatar/2.jpeg"
        },
        {
          id: 2,
          nombre: "Rick",
          imagen: "https://rickandmortyapi.com/api/character/avatar/1.jpeg"
        },
        {
          id: 3,
          nombre: "Summer",
          imagen: "https://rickandmortyapi.com/api/character/avatar/3.jpeg"
        },
        {
          id: 4,
          nombre: "Beth",
          imagen: "https://rickandmortyapi.com/api/character/avatar/4.jpeg"
        },
        {
          id: 5,
          nombre: "Jerry",
          imagen: "https://rickandmortyapi.com/api/character/avatar/5.jpeg"
        }
      ]
        }
    }
}
</script>