<template>
    <section> 
        <div style="display: flex" class="contenedor container">
            <div>
                <div class="circulos">
                    <div style="background:#28a745" class="circulo"></div>
                    <div style="background:#f33d33" class="circulo"></div>
                    <div style="background:#007cc6" class="circulo"></div>
                    <div style="background:#ffcc33" class="circulo"></div>
                </div>
                <div class="textos">
                    <h1>Evoluciona hacia un <span>crecimiento exponencial</span></h1>
                    <h2>Descubre los contenidos que hemos preparado para que hagas crecer tu negocio de manera sostenible.</h2>
                </div>
            </div>
            <div class="rojo_bci">
                <div class="logo_master">
                    <div  class="circunferencia1"></div>
                    <div  class="circunferencia2"></div>
                </div>
                <img src="../assets/img/rojo.png" alt="bci_rojo">
                <div style="margin: -220px 0 0 -30px" class="botones">
                    <card
                        text="Ver calendarios"
                        icon="calendar"
                        type='is-success'
                    >
                    </card>

                    <card
                        text="Eventos anteriores"
                        icon="clock"
                        type="is-info"
                    >
                    </card>
                </div>
                <div style="margin: -220px 0 0 410px" class="botones">
                    <card
                        text="Santiago"
                        icon="home"
                        type="is-danger"
                    >

                    </card>

                    <card
                        text="Regiones"
                        icon="city"
                        type="is-warning"
                    >
                    </card>
                </div>
            </div>
        </div>
    </section>
</template>
<script>
import card from './Card'

export default {
    name:"Banner",
    components:{
        card
    }
}
</script>
<style lang="scss" scoped>
    section{
        width: 100vw;
    }
    .conntenedor{
        height: 500px;
        
        
    }
    .circulos{
        margin: 60px 0 10px 5px;
        display: grid;
        grid-template-columns: repeat(4,1fr);
        width: 60px ;
        .circulo{
            width: 5px;
            height: 5px;
            background: rgb(246, 156, 85);
            border-radius: 50%;
        }
    }
    
    .textos{
        width: 540px;
        margin: 10px 0 0 0;
        h1{
            color: rgb(84, 110, 122);
            font-size: 40px;
            margin-bottom: 10px;
            line-height: 1
        }
        span{
            color: #28a745;
            font-weight: 600
        }
        h2{
            margin: 0 80px 150px 0 ;
            opacity: 0.78;
        }
    }
    
    img{
        height: 350px;
        width: auto;
        position: absolute;
        margin: -310px 0 0 100px
    }
    
    .logo_master{
        display: grid;
        grid-template-columns: repeat(2,1fr);
        margin: 14% 0 0 35%;
        .circunferencia1{
            width: 250px;
            height: 250px;
            z-index: -1;
            position: relative;
            border: 2px #999999 solid;
            opacity: 0.4;
            border-radius: 50%;
            margin: -60px 0 0 -120px
        }
        .circunferencia2{
            width: 250px;
            height: 250px;
            z-index: -1;
            position: relative;
            border: 2px #999999 solid;
            opacity: 0.4;
            border-radius: 50%;
            margin: -60px 0 0 -180px
        }
    }

    .rojo_bci{
        margin-left: 2vw
    }
    
</style>