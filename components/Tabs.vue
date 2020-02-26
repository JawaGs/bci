<template>
   <div class="container">
          <section>
            <h1>Proximos Eventos</h1>    
            <b-tabs position="is-right">
                  <b-tab-item label="MARKETING">
                        <div class="contenedor_cartas">
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              
                        </div>
                  </b-tab-item>

                  <b-tab-item label="NEGOCIOS">
                        <div class="contenedor_cartas">
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>

                        </div>
                  </b-tab-item>

                  <b-tab-item  label="LIDERAZGO">
                        <div class="contenedor_cartas">
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              

                        </div>
                  </b-tab-item>

                  <b-tab-item label="CAPACITACIONES" >
                        <div class="contenedor_cartas">
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                              <CardTabs texto="Lorem ipsum dolor sit amet consectetur adipisicing elit. " fecha="sab., mar.21, 10:00" titulo="Nombre Evento"  imagen='https://images.pexels.com/photos/3626622/pexels-photo-3626622.jpeg?auto=compress&cs=tinysrgb&dpr=2&h=650&w=940'/>
                             
                              

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
      h1{
            font-size: 40px;
            margin: 0 0 -40px 10px;
            font-weight: 400;
            color: #606060
      }
</style>
