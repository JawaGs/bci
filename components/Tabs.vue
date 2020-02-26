<template>
   <div class="container">
          <section>

            <b-tabs position="is-right">
                  <b-tab-item label="MARKETING">
                        <div class="contenedor_cartas">
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>

                        </div>
                  </b-tab-item>

                  <b-tab-item label="NEGOCIOS">
                        <div class="contenedor_cartas">
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>

                        </div>
                  </b-tab-item>

                  <b-tab-item  label="LIDERAZGO">
                        <div class="contenedor_cartas">
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              

                        </div>
                  </b-tab-item>

                  <b-tab-item label="CAPACITACIONES" >
                        <div class="contenedor_cartas">
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs text="Esta es una prueba" imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                             
                              

                        </div>
                  </b-tab-item>
            </b-tabs>
      </section>
   </div>
</template>

<script>
import CardTabs from './Card_Tabs'

    export default {
          name:"Tabs",
          components:{
            CardTabs
          },
        data() {
            return {
                activeTab: 0,
                showBooks: false
            }
        }
    }
</script>
<style lang="scss" scoped>
      .contenedor_cartas{
            display: grid;
            grid-template-columns: repeat(4,1fr)
      }
</style>
