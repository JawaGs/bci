<template>
  <div class="column">
    <div  class="card"> 
      <label class="fecha">{{ fecha }}</label>
      <label class="titulo">{{ titulo }}</label>
      <label class="texto">{{ texto }}</label>
      <label class="link">
        <nuxt-link to="/1">MAS INFORMACION <b-icon icon="plus-circle" size="is-small" /></nuxt-link>
      </label>
      <div class="card-image">
        <img :src="imagen" alt="Logo">
        <div class="overlay"></div>
        
      </div>
      
    </div>
  </div>
</template>

<script>
export default {
  name:"CardTabs" ,   
  props: {
    fecha: {
      type: String,
      required: true
    },
    titulo: {
      type: String,
      required: true
    },
    texto: {
      type: String,
      required: true
    },
    imagen: {
      type: String,
      required: true
    },
  }
}
</script>
<style lang="scss" scoped>
  
  .card{
    width: 100%;
    height: 400px;
    font-size: 12px;
    border-radius: 10px;
    transition: all 0.1s ease-out;
    -webkit-box-shadow: 0px -1px 18px -3px rgba(0,0,0,0.7);
    -moz-box-shadow: 0px -1px 18px -3px rgba(0,0,0,0.7);
    box-shadow: 0px -1px 18px -3px rgba(0,0,0,0.7);
   

    img{
          height: 400px;
          width: 100%;
          opacity: 0.8;
    }
    .overlay{
          height: 400px;
          width: 100%;
          margin: -400px 0 0 0 ;
          z-index: 2;
          position: absolute;
            background: #000;  /* fallback for old browsers */
            background: -webkit-linear-gradient(to top, #000, transparent);  /* Chrome 10-25, Safari 5.1-6 */
            background: linear-gradient(to top, #000, transparent); /* W3C, IE 10+/ Edge, Firefox 16+, Chrome 26+, Opera 12+, Safari 7+ */
    }
    
    .fecha{
      position: absolute;
      z-index: 3;
      color: white;
      font-size: 14px;
      margin: 250px 30px 0 30px;
    }
    .titulo{
      position: absolute;
      z-index: 3;
      color: white;
      font-size: 20px;
      margin: 270px 30px 0 30px;
      font-weight: 600
    }
    .texto{
      position: absolute;
      z-index: 3;
      color: white;
      font-size: 16px;
      margin: 300px 30px 0 30px
    }
    .link{
      position: absolute;
      z-index: 3;
      color: white;
      font-size: 20px;
      margin: 355px 30px 0 30px;
      a{
        color: azure
      }
      
    }
  }

</style>
