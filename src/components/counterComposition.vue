<template>
    <div>
        <h3>{{conuter}}</h3>
        <button @click="addCount">Incrementar</button>    
    </div>
</template>

<script lang="ts">
import { defineComponent, ref } from 'vue';
export default defineComponent({
    name: 'contadorComposition',
    setup(){ 
        let conuter = ref(0);
        const addCount = () => {
            conuter.value++;
        }
        return{conuter, addCount}
    }
})
</script>