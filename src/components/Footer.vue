<template>
    <div>
        <footer>
            <div class="footer-container bg-dark">
                <div class="footer-main">
                    <div class="footer-columna">
                        <h3>Nuestra empresa</h3>
                        <ul>
                            <li><span><p>Terminos y condiciones</p></span></li>
                            <li><span><p>El Salvador</p></span></li>
                            <li><span><p>&copy; 2020, Todos los derechos reservados</p></span></li>
                        </ul>
                    </div>
                    <div class="footer-columna">
                        <h3>Direccion</h3>
                        <ul>
                            <li><span><p>224 Av. Garrobo San Miguel - El Salvador</p></span></li>
                            <li><span><p>(+503) 7777-7777</p></span></li>
                            <li><span><p>outsurcing@sanmiguel.com</p></span></li>
                        </ul>
                    </div>
                    <div class="footer-columna">
                        <h3>Redes sociales</h3>
                        <p>Facebook</p>
                        <p>Instagram</p>
                        <p>Twieter</p>
                    </div>
                </div>
            </div>
        </footer>
    </div>
</template>

<script>
    export default {
        name: "Footer"
    }
</script>

<style>
    *{
        margin: 0;
        padding: 0;
        -webkit-box-sizing: border-box;
        -moz-box-sizing: border-box;
        box-sizing: border-box;
    }
    ul li{
        list-style: none;
    }
    footer{
        width: 100%;
        font-family: "Agency FB";
    }
    .footer-container{
        width: 100%;
        color: white;
    }
    .footer-main{
        width: 98%;
        max-width: 1000px;
        margin: auto;
        padding: 50px 0px;
        display: flex;
        flex-wrap: wrap;
    }
    .footer-main .footer-columna{
        width: calc(100% / 3);
        text-align: justify;
    }
    .footer-main .footer-columna:nth-child(2){
        padding: 0px 20px;
    }
    .footer-main .footer-columna h3{
        font-size: 32px;
        color: #42b983;
    }
    .footer-main .footer-columna span p{
        display: inline-block;
        margin-left: 5px;
        margin-bottom: 15px;
    }
    @media screen and (max-width: 750px){

        .footer-main .footer-columna{
            padding: 0 10px;
        }
        .footer-main .footer-columna h3{
            font-size: 28px;
        }
        .footer-main .footer-columna p{
            font-size: 14px;
        }
    }

    @media screen and (max-width: 640px){
        .footer-main .footer-columna{
            width: 100%;
            text-align: center;
            margin: 10px 0px;
        }
        .footer-main .footer-columna h3{
            margin-bottom: 5px;
        }
        .footer-main .footer-columna span{
            display: block;
        }
    }
</style>