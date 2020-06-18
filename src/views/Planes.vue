<template>
    <div >
        <div class="contenedor">
            <h1>Elije tu plan de suscripsción</h1>
            <h5>Disfruta de una herramienta capaz de aumentar la eficiencia de tu negocio o empresa</h5>
        </div>

        <div class="row">
            <div class="col-sm-1"></div>
            <div class="planes col-sm-4">
                <h5 class="text-center">Sucripción mensual</h5>
                <img src="../assets/DineroLogo.png" width="400" height="400" class="image">
                <div class="overlay bg-dark" >
                    <div class="text">
                        Suscripcion mensual
                        <b-button block pill variant="success">Comprar</b-button>
                    </div>
                </div>
            </div>
            <div class="col-sm-2"></div>
            <div class="planes col-sm-4">
                <h5 class="text-center">Sucripción anual</h5>
                <img src="../assets/DineroLogo.png" width="400" height="400" class="image">
                <div class="overlay bg-dark" >
                    <div class="text">
                        Suscripcion anual
                        <b-button block pill variant="success">Comprar</b-button>
                    </div>
                </div>
            </div>
            <div class="col-sm-1"></div>
        </div>

        <div class="contenedor">
            <h1>¿Porque pagar la suscripción?</h1>
            <h5>Tendras acceso a los diferentes modulos disponibles</h5>
        </div>

        <Footer/>
    </div>
</template>

<script>
    import Footer from "@/components/Footer";
    export default {
        name: "Planes",
        components:{Footer}
    }
</script>

<style>

    .contenedor{
        text-align: center;
        margin: auto;
        width: 90%;
        font-family: 'Open Sans', sans-serif;
    }

    div.row{
        margin-right: 0px;
        padding: 2rem 0rem;
    }

    .planes{
        position: relative;
        border-radius: 5px 5px 5px 5px;
        box-shadow: 5px 5px 5px 0px rgba(0,0,0,0.75);
    }
    .image {
        display: block;
        margin: auto;
    }

    .overlay {
        margin: auto;
        position: absolute;
        bottom: 0;
        left: 0;
        right: 0;
        border-radius: 5px 5px 5px 5px;
        overflow: hidden;
        height: 0;
        transition: .5s ease;
        opacity: 0.99;
    }

    .planes:hover .overlay {
        height: 100%;
    }

    .text {
        color: white;
        font-size: 20px;
        position: absolute;
        top: 50%;
        left: 50%;
        -webkit-transform: translate(-50%, -50%);
        -ms-transform: translate(-50%, -50%);
        transform: translate(-50%, -50%);
        text-align: center;
    }

</style>