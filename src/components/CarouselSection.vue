<template>
            <!-- carousel -->
        <div id="carouselExampleCaptions" class="carousel slide" data-ride="carousel">
            <ol class="carousel-indicators">
                <li data-target="#carouselExampleCaptions" data-slide-to="0" class="active"></li>
                <li data-target="#carouselExampleCaptions" data-slide-to="1" class=""></li>
                <li data-target="#carouselExampleCaptions" data-slide-to="2" class=""></li>
            </ol>
            <div class="carousel-inner">
                <div class="carousel-item active">
                    <img src="https://i.ibb.co/pdcyNYm/2Ovcka3.jpg" class="d-block w-100" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Ultimo modelo de David Fender X600</h5>
                        <p>El 31 de diciembre saldra a la venta la ueva X600 de David Fender</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="https://i.ibb.co/3NCSNLP/82af286ea16f6e2299651ebc986c2af5.jpg" class="d-block w-100" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Vetnas de las guitarras David Fender se increentan en Pandemia</h5>
                        <p>las vetas de David Fender aumentaron un 17% durante la pandemia alcnaznado un total de 700 millones de dolares en ventas.</p>
                    </div>
                </div>
                <div class="carousel-item">
                    <img src="https://i.ibb.co/6vfbVd7/download.jpg" class="d-block w-100" alt="...">
                    <div class="carousel-caption d-none d-md-block">
                        <h5>Third slide label</h5>
                        <p>Praesent commodo cursus magna, vel scelerisque nisl consectetur.</p>
                    </div>
                </div>
            </div>
            <a class="carousel-control-prev" href="#carouselExampleCaptions" role="button" data-slide="prev">
                <span class="carousel-control-prev-icon" aria-hidden="true"></span>
                <span class="sr-only">Previous</span>
            </a>
            <a class="carousel-control-next" href="#carouselExampleCaptions" role="button" data-slide="next">
                <span class="carousel-control-next-icon" aria-hidden="true"></span>
                <span class="sr-only">Next</span>
            </a>
        </div>
    
</template>
<script>

    export default {
        name: "CarouselSection",
        
    };
</script>

<style>
.carousel-inner{
  width:100%;
  max-height: 600px !important;
}
</style>

