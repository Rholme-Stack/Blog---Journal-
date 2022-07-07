<template>
    <div class="d-flex justify-content-center">
        <button class="btn btn-secondary">
            <i :class="icon"></i>
            
          

        </button>

    </div>
    
</template>

<script lang="ts">
export default{
        props:{
            icon:{
                type:String,
                default:'bi bi-file-earmark-plus'

            }
        }

}

</script>

<style lang="scss" scoped>

button{
    position: fixed;
    bottom: 20px;
    right: 20px;
    width: 50px;
    height: 50px;
    border-radius: 100% ;
    


}
i{
    size:30px
}

</style>