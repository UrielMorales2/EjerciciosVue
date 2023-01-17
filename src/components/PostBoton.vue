<template>
    <div>
       <button class="post-btn">ACCEDER</button> 
    </div>
</template>

<script lang="ts">
export default ({
  name: 'PostBoton',
});
</script>



<style scoped>
.post-btn {
    padding: 15px;
    background-color: blueviolet;
    color: #fff;
    border: 0;
    outline: 0;
}
.post-btn:hover {
    background-color: #fff;
    color: blueviolet;
}
</style>