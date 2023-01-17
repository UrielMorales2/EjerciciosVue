<template>
  <!-- <conuter_option></conuter_option>
  <contadorComposition></contadorComposition>
  <h1>Listado de Post</h1>
  <PostContainer></PostContainer> -->
  <!-- <directivasSelectivas></directivasSelectivas> -->
  
  <ModelForm></ModelForm>

</template>


<script lang="ts">
import conuter_option from './components/ContadorOption.vue'
import PostContainer from './components/PostContainer.vue';
import contadorComposition from './components/counterComposition.vue';
import directivasSelectivas from './components/directivasSelectivas.vue';
import ModelForm from './components/ModelForm.vue';
export default ({
  name: 'App',
  components: {
    // PostContainer,
    // conuter_option, 
    // contadorComposition,
    // directivasSelectivas,
    ModelForm,
  }
});
</script>

<style>

</style>
