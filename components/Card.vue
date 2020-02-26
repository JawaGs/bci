<template>
  <div class="column">
    <div class="card">
     
      <div class="card-content icono">
        
          <b-icon
            
            :icon="icon"
            size="is-medium"
            :type="type"
          />
          <p>{{text}}</p>
        
      </div>
     
    </div>
  </div>
</template>

<script>
export default {
  props: {
    text: {
      type: String,
      required: true
    },
    type: {
      type: String,
      required: true
    },
    icon: {
      type: String,
      required: true
    },
    
  }
}
</script>
<style lang="scss" scoped>
  .icono{
    display: flex
  }
  
  .card{
    width: 230px;
    height: 70px;
    font-size: 12px;
    border-radius: 10px;
    transition: all 0.1s ease-out;
    -webkit-box-shadow: 0px -1px 18px -3px rgba(0,0,0,0.7);
    -moz-box-shadow: 0px -1px 18px -3px rgba(0,0,0,0.7);
    box-shadow: 0px -1px 18px -3px rgba(0,0,0,0.7);
    p{
      margin: 5px 0 0 10px
    }
    i{
      font-size: 1px
    }
  }

</style>
