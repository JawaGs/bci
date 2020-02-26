<template>
    <section class="container">
        <div class="columns is-desktop">
            <div class="column">
                Aqui va el mapa 
            </div>
            <div class="column">
                <div class="circulos">
                    <div style="background:#28a745" class="circulo"></div>
                    <div style="background:#f33d33" class="circulo"></div>
                    <div style="background:#007cc6" class="circulo"></div>
                    <div style="background:#ffcc33" class="circulo"></div>
                </div>
                <h1>
                    Detalle contenido
                </h1>
                <section>
                    <div class="content">
                        
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <br/>
                            Nulla accumsan, metus ultrices eleifend gravida, nulla nunc varius lectus, nec rutrum justo nibh eu lectus. <br/>
                            Ut vulputate semper dui. Fusce erat odio, sollicitudin vel erat vel, interdum mattis neque.
                        </p>
                        <p>
                            Lorem ipsum dolor sit amet, consectetur adipiscing elit. <br/>
                            Nulla accumsan, metus ultrices eleifend gravida, nulla nunc varius lectus, nec rutrum justo nibh eu lectus. <br/>
                            Ut vulputate semper dui. Fusce erat odio, sollicitudin vel erat vel, interdum mattis neque.
                        </p>
                        <h4>Los pilares del contenido son:</h4>
                        <ul>
                            <li class="elemento">- Emprendimiento</li>
                            <li class="elemento">- Tendencia y desarrollo digital</li>
                            <b-collapse class="acordeon" :open="false" position="is-bottom" aria-id="contentIdForA11y1">
                                <a slot="trigger" slot-scope="props" aria-controls="contentIdForA11y1">
                                    {{ !props.open ? 'VER TODO EL CONTENIDO ' : 'VER MENOS CONTENIDO' }}
                                    <b-icon :icon="!props.open ? 'plus-circle-outline' : 'minus-circle-outline'"></b-icon>
                                </a>
                                <li class="elemento">- Desarrollo personal</li>
                                <li class="elemento">- Educacion digital</li>
                                <li class="elemento">- Marketing digital</li>
                                
                            </b-collapse>
                            
                        </ul>
                    </div>
                    <div class="speaker is-flex">
                        <img src="../assets/img/speaker.jpg" alt="speaker_photo">
                        <div class="speaker_data">
                            <h5>Speaker: John Doe</h5>
                            <p>Lorem ipsum dolor sit amet consectetur.  </p>
                        </div>
                    </div>
                </section>
            </div>
        </div>
        <div class="card is-flex">
            <span></span>
            <p>Martes 20 de Febrero de 2020, 11:00</p>
            <p><strong>Total: </strong> Gratis </p>
            <button @click="isCardModalActive = true" class="boton">REGISTRARME AL EVENTO</button>
        </div>
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
                                    <b-input size='is-medium' v-model="datos.nombre" required class="campo" name="nombre"  ></b-input>
                                </b-field>
                                <label for="apellido">Apellido</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.apellido" required class="campo" name="apellido"  ></b-input>
                                </b-field>
                                <label for="rut">Rut</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.rut" required name="rut"  class="campo" ></b-input>
                                </b-field>
                                <label for="nombre_empresa">Nombre Empresa</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.nombre_empresa" required name="nombre_empresa" class="campo"  ></b-input>
                                </b-field>
                                <label for="rut_empresa">Rut Empresa</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.rut_empresas" required name="rut_empresa"  class="campo" ></b-input>
                                </b-field>
                                <label for="numero">Numero de Personas</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.numero" required type='number' max='2' name="numero"  class="campo" ></b-input>
                                    
                                </b-field>
                                
                                <label for="email">Correo Electronico</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.email" required type="email" class="campo" name="email"  ></b-input>
                                </b-field>
                                <label for="phone">Telefono</label>
                                <b-field  >
                                    <b-input size='is-medium' v-model="datos.telefono" type='number' required name="phone" class="campo" ></b-input>
                                </b-field>
                                
                                <button class="boton_registrarse"><nuxt-link to="/resumen">REGISTRARME AHORA</nuxt-link></button>
                            </form>
                            
                    </div>
                </b-modal>
            </section>
        </template>
    </section>
</template>
<script>

export default {
    name:"Eventos",
        data() {
            return {
                datos:{
                    nombre:'',
                    apellido:'',
                    rut:'',
                    nombre_empresa:'',
                    rut_empresas:'',
                    numero:'',
                    email:'',
                    telefono:''
                },
                isCardModalActive: false
            }
        },
        watch:{
            isCardModalActive:function(){
                console.log(this.datos)
            }
        }
}
</script>
<style lang="scss" scoped>
    .container{
        margin-top: 50px;
        
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
        h1{
            font-size: 42px;
            color: #505050
        }
        ul{
            li{
                list-style: none;
            }
        }
        .acordeon{
            margin-top: 15px
        }
        .speaker{
            margin: 60px 0;
            img{
                width: 60px;
                border-radius: 50%;
            }
            .speaker_data{
                margin: 10px  0 0 10px;
                    h5{
                        font-weight: 600
                    }
                }
        }
        .card{
            margin-bottom: 100px;
            height: 80px;
            span{
                width: 5px;
                background-color: #28a745
            }
            button{
                background-color: #28a745;
                color: whitesmoke;
                font-size: 16px;
                font-weight: 600;
                border: none;
                padding: 15px 30px;
                margin: 10px 0 0 70px;
                border-radius: 24px;
                height: 60px;
            }
            p{
                font-size: 24px;
                margin: 20px 0 0 30px;
                strong{
                    margin-left: 400px
                }
            }
        }
        .form_modal{
            height: 980px;
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
                font-size: 24px
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
                a{
                    color: white
                }
            }
        } 

    }
</style>