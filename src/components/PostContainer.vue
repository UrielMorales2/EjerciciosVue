<template>
    <div class="post-container">
        <PostCard />
        <PostCard />
        <PostCard />
        <PostCard />
    </div>
</template>



<script lang="ts">
import PostCard from './PostCard.vue';

export default ({
  name: 'PostContainer',
  components: {
    PostCard
  }
});
</script>









<style scoped>
.post-container{
    width: 100%;
    display: flex;
    flex-wrap: wrap;
}
</style>