<!-- directivas selectivas (renderizado  condicional) -->

<template>
    <h1 v-if="edad < 18">eres menor de edad</h1>
    <h2 v-else >eres mayor de edad</h2>


    <ul>
        <li v-for="pais in paises" :key="pais">   {{ pais }}</li>
    </ul>

    <ul>
        <li v-for="nombre in nombres" :key="nombre.code">
            {{ nombre.name }}
        </li>
    </ul>



    <p v-bind:class="{'danger':hasError}">El mensaje se ha enviado satisfactoriamente</p>

    <p v-bind:style="{'background-color' : '#ccc', color: c}" >hola mundo v-bind por estilos</p>

    <!-- ---------------- v-on --------------------- -->
    <button v-on:click="cambiarColor()">Cambiar color</button>





</template>

<script lang="ts" setup>
    
    import { Ref, ref } from 'vue';
    
    let edad = 19;
    
    let paises:Ref<Array<string>> = ref([
        'mexico', 'italia', 'Canda', 'Francia', 'Colombia'
    ]);

    interface INombres {
        code: string,
        name: string,
        cel: number;
    }

    let nombres:Ref<Array<INombres>> = ref ([
        {
            code: 'es',
            name: 'david',
            cel: 987654
        },
        {
            code: 'es',
            name: 'carlos',
            cel: 987654
        },
        {
            code: 'es',
            name: 'Karen',
            cel: 987654
        },
        {
            code: 'es',
            name: 'andrea',
            cel: 987654
        },
        {
            code: 'es',
            name: 'Lupe',
            cel: 987654
        }
    ])


    // -----para el v-bing
    let hasError = true; 


    // ------------- v-on---------------
        let c = ref('#fff');

        const cambiarColor = () => {c.value = '#ff0000'};


</script>


<style scoped> 
.danger{
    color : red;
}
</style>