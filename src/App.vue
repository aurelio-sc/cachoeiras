<template>
  <div>
    <h1>{{ title }}</h1>
    <ul class="waterfallList">
    <li class="waterfall" v-for="waterfall of waterfalls" :key="waterfall.id">
      <h2 class="waterfallName">{{ waterfall.name }} </h2>
      <img :src="waterfall.source" :alt="waterfall.name">
      <p class="textContent">{{ waterfall.location }}</p>
      <p class="textContent">{{ waterfall.description }}</p>
    </li>
    </ul>
    
  </div>
</template>

<script>
export default {
  
  data () {
    return {
      title: 'Cachoeiras do Espírito Santo',

      waterfalls: [
        { 
          name: 'Cachoeira Alta',
          source: './src/assets/img/cachoeiraAlta.jpg',          
          location: 'Cachoeiro de Itampemirim',
          description: 'Com águas cristalinas e uma queda de apoximadamente 100 metros, é um ótimo local para amantes da fotografia. Contém um bar no qual é possível fazer um churrasco caso o visitante consuma no local.'
        },

        {
          name:'Cachoeira Arco Íris',
          source: './src/assets/img/cachoeiraArcoIris.jpg',
          loacation: 'Divino de São Lourenço',
          description: 'Localizada no Patrimônio da Penha, faz parte de um complexo de cascatas, juntamente com a Cachoeira do Beija-Flor e a cachoeira da Vó Tuti. Na última de suas quedas (são quatro!) possui um lindo poço que se assemelha a uma piscina. É possível acampar nas proximidades.'
        }
      ]

    }
  }
}
</script>

<style>

</style>
