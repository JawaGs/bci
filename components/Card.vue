<template>
  <div class="column">
    <div class="card">
     
      <div class="card-content icono">
        
          <b-icon
            
            :icon="icon"
            size="is-large"
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
<style lang="css" scoped>
  .icono{
    display: flex
  }
  p{
    margin: 12px
  }
  .card{
    width: 310px;
    border-radius: 10px;
    transition: all 0.1s ease-out;
    padding: 0px 0
  }
  .card:hover{
    width: 320px;
    padding: 0 25px 0 0
  }
</style>
