<template>
    <div class="post-card">
        <h3>Titulo</h3>
        <p>Lorem ipsum dolor sit amet, consectetur adipisicing elit. Voluptatem totam in ad aliquid sequi officia, at dolorem iusto molestiae similique, inventore illo ducimus distinctio labore incidunt voluptas. Magni, sunt impedit.</p>
        <PostBoton></PostBoton>
    </div>
</template>

<script lang="ts">
import PostBoton from './PostBoton.vue';

export default ({
  name: 'PostCard',
  components: {
    PostBoton
  }
});
</script>

<style scoped>
.post-card{
    border-radius: 15px;
    padding: 10px;
    margin: 5px;
    border: 1px solid #ccc;
}
</style>