<template>
  <!-- <conuter_option></conuter_option>
  <contadorComposition></contadorComposition>
  <h1>Listado de Post</h1>
  <PostContainer></PostContainer> -->
  <directivasSelectivas></directivasSelectivas>
</template>


<script lang="ts">
import conuter_option from './components/ContadorOption.vue'
import PostContainer from './components/PostContainer.vue';
import contadorComposition from './components/counterComposition.vue';
import directivasSelectivas from './components/directivasSelectivas.vue';
export default ({
  name: 'App',
  components: {
    // PostContainer,
    // conuter_option, 
    // contadorComposition,
    directivasSelectivas
  }
});
</script>

<style>
h1{
    color: green;
}
</style>
