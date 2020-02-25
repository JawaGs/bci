<template>
    <section> 
        <div style="display: flex" class="contenedor">
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
            <div class="rojo_bi">
                <div class="logo_master">
                    <div style="marginLeft: -90px; marginTop:-60px" class="circunferencia"></div>
                    <div style="marginLeft: -250px; marginTop:-58px" class="circunferencia"></div>
                </div>
                <img src="../assets/img/rojo.png" alt="bci_rojo">
                <div style="margin: -280px 0 0 -40px" class="botones">
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
                <div style="margin: -270px 0 0 520px" class="botones">
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
<style lang="css" scoped>
    section{
        width: 100vw;
    }
    .conntenedor{
        height: 500px;
        width: 60% !important;
        
    }
    .circulos{
        margin: 10% 0 0.5% 18.5%;
        display: grid;
        grid-template-columns: repeat(4,1fr);
        width: 7% 
    }
    .circulo{
        width: 5px;
        height: 5px;
        background: rgb(246, 156, 85);
        border-radius: 50%;
    }
    .textos{
        width: 73.5%;
    }
    h1{
        color: rgb(84, 110, 122);
        font-size: 40px;
        margin: 0 0 5% 25%;
        line-height: 1
    }
    span{
        color: #28a745;
        font-weight: 600
    }
    h2{
        margin: 1% 0 0 25%;
        opacity: 0.78;
    }
    img{
        height: 400px;
        position: absolute;
        margin: -18% 0 0 8%
    }
    .circunferencia{
        width: 250px;
        height: 250px;
        z-index: -1;
        position: relative;
        border: 2px #999999 solid;
        opacity: 0.4;
        border-radius: 50%;
    }
    .logo_master{
        display: grid;
        grid-template-columns: repeat(2,1fr);
        margin: 14% 0 0 35%
    }
    .botones .card{
        margin: 10px 0;
        width: 250px;
        padding: 15px 0 15px 10px;
        text-align: center
    }
</style>