<template>
    <div class="container contenedor">
        <nuxt-link to="/"><b-icon icon="arrow-left" size="is-small" /> Volver a todos a los eventos</nuxt-link>
        <h1> Resumen registro</h1>
        <h2>Descargar las entradas de tu evento</h2>
        <div class="card is-flex">
            <span></span>
            <div class="textos">
                <strong><p>Conferencia de negocios inteligentes en Internet.</p></strong>
                <p >Martes 20 de Febrero de 2020, 11:00 </p>
            </div>
            <button @click="isCardModalActive = true" class="boton">DESCARGAR ENTRADAS</button>
        </div>
        <div class="has-background-white-ter">
            <h3>
                Orden #123456
            </h3>
        </div>
        <div class="columns is-desktop">
            <div class="column">
                <div class="columns is-desktop">
                    <div class="column">
                        <label for="nombre">Nombre:</label>
                        <p name="nombre">xxx</p>
                        <label for="nombre_empresa">Nombre de Empresa:</label>
                        <p name="nombre_empresa">xxxxxxx</p>
                        <label for="numero">Numero de Entradas:</label>
                        <p name="numero">10</p>
                    </div>
                    <div class="column">
                        <label for="nombre">Mail:</label>
                        <p name="nombre">xxx</p>
                        <label for="nombre_empresa">Fecha de Registro:</label>
                        <p name="nombre_empresa">xxxxxx</p>
                        <label for="numero">Total</label>
                        <p name="numero">Gratis</p>
                    </div>
                </div>   
            </div>
            <div class="column">Aqui va el mapa</div>
        </div>
    </div>
</template>
<style lang="scss" scoped>
    .contenedor{
        margin-top: 50px;
        h1{
            color: #606060;
            font-size: 40px
        }
        h2{
            margin-top: 20px
        }
        h3{
            font-size: 20px;
            font-weight: 600
        }
        .has-background-white-ter{
            padding: 15px;
            margin-bottom: 60px
        }
        .card{
            margin-bottom: 30px;
            height: 80px;
            span{
                width: 5px;
                background-color: #28a745
            }
            button{
                background-color: #28a745;
                color: whitesmoke;
                font-size: 14px;
                font-weight: 600;
                border: none;
                padding: 15px 30px;
                margin: 10px 0 0 700px;
                border-radius: 24px;
                height: 60px;
            }
            .textos{
                margin: 15px 0 0 30px;
                p{
                    color: #606060;
                    font-size: 14px
                }
            }
        }
        label{
            font-weight: 600;

        }
        .column{
            p{
                margin: 0 0 30px 0
            }
        }
    }
</style>