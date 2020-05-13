<template lang="html">

  <div v-if='country' class="country-details">
      <h3>{{country.name}}</h3>
      <p>Population: {{country.population}}</p>
      <p>Main Language spoken: {{country.languages[0].name}}</p>
      
  </div>
</template>

<script>
import { eventBus } from '../main.js';

export default {
    name: 'country-detail',
    props: ['country']
}
</script>

<style>
  .country-details{
  position: fixed;
  top: 0;
  right:20%;
    }


</style>