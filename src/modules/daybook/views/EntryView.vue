<template>
  <div class="entry-title d-flex justify-content-between p-2">
    <div>
      <span class="text-success fs-3 fw-bold">14</span>
      <span class="mx-1 fs-3">Julio</span>
      <span class="mx-2 fs-4 fw-light">2022, jueves</span>
      </div>

      <div>
        <button class="btn btn-danger mx-2">
          Borrar
          <i class="bi bi-trash"></i>
        </button>
        <button class="btn btn-secondary">
          Subir Foto  
            <i class="bi bi-upload"></i>
          
        </button>


      </div>


  </div>

  <hr>
  <div class="d-flex flex-column px-3  h-75">
    <textarea name="" id="" cols="" rows="" placeholder="¿Como ha sido tu día?"></textarea>

  </div>

 <FabBoton icon="bi bi-save"/>


 <img src="https://teambike.com/wp-content/uploads/teambike-equipo.jpg" 
      alt="entry-img"
      class="img-thumbnail">
      
</template>

<script lang="ts">
import { defineAsyncComponent } from "vue"

export default {
  components:{
      FabBoton: defineAsyncComponent(()=> import('../components/FabBoton.vue'))

  }

}
</script>

<style lang="scss" scoped>
textarea{
  font-size: 20px;
  border: none;
  height: 100%;


    &:focus{
    outline: none;
  }
}

img{
  width: 300px;
  position: fixed;
  bottom: 100px;
  right: 20px;
  box-shadow: 0px 5px 10px rgba($color: #000000, $alpha: 0.2);

}

</style>