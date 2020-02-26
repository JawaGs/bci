<template>
    <div class="contenedor">
        <BannerEventos  />
        <Eventos />
    </div>
</template>
<script>
import BannerEventos from "../components/Banner_Eventos"
import Eventos from "../components/Eventos"

export default {
    components:{
        BannerEventos,
        Eventos
    } ,
    data(){
    
    },

}
</script>
<style lang="scss" scoped>
    .contenedor{
        width: 100vw !important
    }
</style>

