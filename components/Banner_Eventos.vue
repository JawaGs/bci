<template>
    <div class="container contenedor">
        
        <nuxt-link to="/"><b-icon icon="arrow-left" size="is-small" /> Volver a todos a los eventos</nuxt-link>
        <h1 class="titulo"> Evento marketing</h1>
        <section class="hero is-medium  has-background-black is-bold">
            <img src="../assets/img/banner.jpg" alt="banner">
            <div class="hero-body">
                
                <div class="container">
                <h1 class="title has-text-centered">
                    Conferencia de Negocios Inteligentes en Internet
                </h1>
                <h2 class="subtitle has-text-centered">
                    Martes 20 de Febrero de 2020, 11:00
                </h2>
                <button  @click="isCardModalActive = true" class="boton">REGISTRARME AL EVENTO</button>
                </div>
            </div>
        </section>
        <template>
            <section>
                <b-modal :active.sync="isCardModalActive">
                    <div class="card form_modal">
                            <div class="circulos">
                                <div style="background:#28a745" class="circulo"></div>
                                <div style="background:#f33d33" class="circulo"></div>
                                <div style="background:#007cc6" class="circulo"></div>
                                <div style="background:#ffcc33" class="circulo"></div>
                            </div> 
                            <h1 class="has-text-centered">Registro de Evento</h1>
                            <form class="container">
                                <label for="nombre">Nombre</label>
                                <b-field  >
                                    <b-input size='is-medium' class="campo" name="nombre"  ></b-input>
                                </b-field>
                                <label for="apellido">Apellido</label>
                                <b-field  >
                                    <b-input size='is-medium' class="campo" name="apellido"  ></b-input>
                                </b-field>
                                <label for="rut">Rut</label>
                                <b-field  >
                                    <b-input size='is-medium' name="rut"  class="campo" ></b-input>
                                </b-field>
                                <label for="nombre_empresa">Nombre Empresa</label>
                                <b-field  >
                                    <b-input size='is-medium' name="nombre_empresa" class="campo"  ></b-input>
                                </b-field>
                                <label for="rut_empresa">Rut Empresa</label>
                                <b-field  >
                                    <b-input size='is-medium' name="rut_empresa"  class="campo" ></b-input>
                                </b-field>
                                <label for="numero">Numero de Personas</label>
                                <b-field  >
                                    <b-input size='is-medium' name="numero"  class="campo" ></b-input>
                                </b-field>
                                <label for="email">Correo Electronico</label>
                                <b-field  >
                                    <b-input size='is-medium' class="campo" name="email"  ></b-input>
                                </b-field>
                                <label for="phone">Telefono</label>
                                <b-field  >
                                    <b-input size='is-medium' name="phone" class="campo" ></b-input>
                                </b-field>
                                <nuxt-link to="/resumen"><button class="boton_registrarse">REGISTRARME AHORA</button></nuxt-link>
                            </form>
                        
                    </div>
                </b-modal>
            </section>
        </template>
    </div>
</template>
<script>
export default {
    name:"BannerEventos",
    data() {
        return {
            isCardModalActive: false
        }
    },
}
</script>
<style lang="scss" scoped>
    .contenedor{
        margin-top: 50px;
        .titulo{
            font-size: 40px;
            color: #606060;
            padding-bottom: 10px;
        }
        h1{
            font-size: 45px;
            color: #fff;
            padding-bottom: 10px;
        }
        h2{
            color: #fff;
            font-size: 24px
        }
        button{
            background-color: #28a745;
            color: whitesmoke;
            font-size: 16px;
            font-weight: 600;
            border: none;
            padding: 15px 30px;
            margin: 0 0 0 520px;
            border-radius: 24px
        }
        img{
            position: absolute;
            opacity: 0.3;
            height: 457px;
            width: 100%
        }
        .form_modal{
            .circulos{
                margin: 10px 0 10px 120px;
                display: grid;
                grid-template-columns: repeat(4,1fr);
                width: 60px ;
                .circulo{
                    width: 7px;
                    height: 7px;
                    background: rgb(246, 156, 85);
                    border-radius: 50%;
                }
        }
            height: 820px;
            width: 450px;
            margin-left: 33%;
            padding: 5px 80px;
            label{
                margin: -13px 0 0 15px;
                position: absolute;
                z-index: 20;
                background-color: white;
                padding: 0px 10px;
                font-weight: 600 ;
                font-size: 18px
            }
            .campo{
                margin: 35px 0;
                font-size: 12px !important
            }
            h1{
                font-size: 24px;
                padding-bottom: 0;
                color: #606060
            }
            .boton_registrarse{
                background-color: #28a745;
                color: whitesmoke;
                font-size: 12px;
                font-weight: 600;
                border: none;
                padding: 0px 30px;
                margin: -15px 0 0 40px;
                border-radius: 24px;
                height: 60px;
            
            }
        } 
    }
</style>