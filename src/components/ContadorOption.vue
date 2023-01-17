    <!-- Primeros Pasos con Option API -->
<template>
    <h3>{{ conter }}</h3>
    <button @click="incrementar();">Incrementar</button>
</template>



<script lang="ts">
    import { defineComponent } from 'vue';
    export default defineComponent({
        name:'conuter_option',
        components:{},
        data(){
            let conter = 0;
            return {conter}
        },
        methods:{
            incrementar(){
                this.conter++;
                console.log("hola mundo");
            },
        }
    })
</script>



<style scoped>

</style>