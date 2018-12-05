<template>
  <div class="home">
    
    <b-container>
      <b-row>
        <b-col v-for="(equipo, index) in equipos" :key='index'>
            <Equipo :info="equipo"/>
        </b-col>
      </b-row>
    </b-container>


   
   
  </div>
</template>

<script>
// @ is an alias to /src

import Equipo from 
"@/components/Equipo.vue";

export default {
  name: 'home',
  components: {
    Equipo
  },
  data(){
      return{
        equipos: [
          {
          nombre: "Equipo 1",
            Logo: "https://via.placeholder.com/600x300/D2B48C/ffffff?text=Logo+equipo",
            estado:true,
            jugadores:[{jugador:"1"},{jugador:"1"}, {jugador:"1"}]
          },
          {
            nombre: "Equipo 2",
            Logo: "https://via.placeholder.com/600x300/D2B48C/ffffff?text=Logo+equipo",
            estado:false,
            jugadores:[{jugador:"1"},{jugador:"1"}]
          },
          {
            nombre: "Equipo 3",
            Logo: "https://via.placeholder.com/600x300/D2B48C/ffffff?text=Logo+equipo",
            estado:true,
            jugadores:[{jugador:"1"},{jugador:"1"}, {jugador:"1"},{jugador:"1"}]
          },
          {
            nombre: "Equipo 4",
            Logo: "https://via.placeholder.com/600x300/D2B48C/ffffff?text=Logo+equipo",
            estado:false,
            jugadores:[]
          }
        ]
      }
  }
}
</script>
