<template>
  <div>
    <h1>{{ title }}</h1>
    <div class="waterfall">
      <h2 class="waterfallName">{{ cachoeiraAlta.name }} </h2>
      <img :src="cachoeiraAlta.source" :alt="cachoeiraAlta.name">
      <p class="textContent">{{ cachoeiraAlta.location }}</p>
      <p class="textContent">{{ cachoeiraAlta.description }}</p>
    </div>
    
  </div>
</template>

<script>
export default {
  
  data () {
    return {
      title: 'Cachoeiras do Espírito Santo',
      cachoeiraAlta: {
        source: "./src/assets/img/cachoeiraAlta.jpg",
        name: 'Cachoeira Alta',
        location: 'Cachoeiro de Itampemirim',
        description: 'Com águas cristalinas e uma queda de apoximadamente 100 metros, é um ótimo local para amantes da fotografia. Contém um bar no qual é possível fazer um churrasco caso o visitante consuma no local.'
      }
    }
  }
}
</script>

<style>

</style>
