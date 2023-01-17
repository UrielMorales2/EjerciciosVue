<template>
    <form action="">
        <input type="text" v-model="inputText"><br>
        <input type="checkbox" v-model="agree">Acepto los Terminos
        <br>
        <select name="" id="" v-model="pais">
            <option value="España">España</option>
            <option value="Francia">Francia</option>
            <option value="Mexico">Mexico</option>            
        </select>
    </form>

    <h3>{{ inputText }}</h3>
</template>

<script lang="ts" setup>
    import {Ref, ref} from 'vue';

    let inputText:Ref<string> = ref('')


    let agree : Ref<boolean> = ref (true);

    let pais :Ref<string> = ref ('Mexico');
    
        
</script>


<style scoped>

</style>