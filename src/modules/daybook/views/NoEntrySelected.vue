<template>
    <div class="d-flex justify-content-center">
        <h1  class="align-self-center">No hay nada seleccionado!</h1>
       <FabBoton/>
    </div>

    

</template>

<script lang="ts">
import { defineAsyncComponent } from 'vue';


export default{
    components:{
        FabBoton: defineAsyncComponent(()=> import('../components/FabBoton.vue'))

    }

}

</script>

<style lang="scss" scoped>
div{

    height: 100%;

}


</style>