<template>
  <div class="column">
    <div  class="card">
      
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
    text: {
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
   

    
    p{
      margin: 5px 0 0 10px;
      
    }
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
    
  }

</style>
