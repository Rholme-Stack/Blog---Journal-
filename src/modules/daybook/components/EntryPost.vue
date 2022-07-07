<template>
<div class="entry-container pointer mb-3 p-2"
    @click="$router.push({name:'entry', params:{id: 10}})"
>
    <div class="entry-title d-flex">
        <span class="text-success fs-5 fw-bold">15</span>
        <span class="mx-1 fs-5">Julio</span>
        <span class="mx-2 fw-light">2021, jueves</span>

    </div>

    <div class="entry-description">
        Consectetur sit in eiusmod irure reprehenderit elit voluptate id sint sit pariatur. Voluptate adipisicing Lorem pariatur aute cupidatat. Sunt sit adipisicing officia enim. Nostrud velit id anim elit proident occaecat consectetur ex deserunt esse nulla. Nisi in laboris et exercitation voluptate.



    </div>

</div>
    
</template>

<script setup lang="ts">

</script>

<style lang="scss" scoped>
.pointer{
cursor:pointer;

}

.entry-description{
border-bottom: 1px solid ;
transition: 0.2s all ease-in;
    &:hover{
        background-color: lighten($color: grey, $amount: 45);
        transition: 0.2s all ease-in;
    }


}

.entry-description{

    font-size: 12px;
}

</style>