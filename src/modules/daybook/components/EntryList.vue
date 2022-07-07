<template>
    <div class="entry-list-container">
        <div class="px-2 pt-2">
           <input type="text"
                  class="form-control"
                  placeholder="Buscar"  
           >        
        </div>

        <div class="entry-scrollarea">
            <EntryPost v-for= "iten in 100"
                :key= "iten">
                Entry card</EntryPost>


        </div>
        
       

    </div>

    
</template>


<script lang="ts" >
import { defineAsyncComponent } from "vue";





export default{
    components: {
        EntryPost: defineAsyncComponent(()=> import('../components/EntryPost.vue')),
        
        
    }
}






</script>

<style lang="scss" scoped>

.imput{
    color: dark;


}
.entry-list-container{
    border-right: 1px solid #2c3e50;
    height: calc(100vh - 56px);
    

   


}

.entry-scrollarea{
    height: calc(100vh - 100px);
    overflow: scroll;
    


}


</style>