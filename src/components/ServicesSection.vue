<template>
        <!-- services -->
    <div class="container-fluid">
            <div class="row justify-content-center mb-5">
                <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
                
                    <div class="card">
                            <div class="d-flex justify-content-center p-2"> 
                                <img src="../assets/GuitarrasElectroAcustica.jpg" alt="" width="100%" height="700px" style="border-radius: 10px;">    
                            </div>
                        <div class="card-body">
                        <h2 class="tiposGuitarraTitulos">
                            Guitarras ElectroAcusticas
                        </h2>
                            <p class="card-text">Estas son las mejores como perfectas guitarras Electroacusticas y al mejor precio del mercado, ya que usamos los mejores 
                            materiales y elementos a la hora de la creacion de nuestras guitarras. Nuestros productos son reconocidos internacionalemente y utilizados
                            por muchos famosos musicos y productores.</p>
                                    <div class="botonTiposGuitarra">
                                        <button type="button" class="btn btn-danger" >Comprar</button>
                                    </div>
                        </div>
                    </div>
                
                </div>
                <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
                    <div class="card">
                        <div class="d-flex justify-content-center p-2">
                            <img src="../assets/GuitarrasAcustica.jpg" alt="" width="100%" height="700px" style="border-radius: 10px;">
                        </div>
                        <div class="card-body">
                        <h2 class="tiposGuitarraTitulos">
                            Guitarras Acusticas
                        </h2>
                            <p class="card-text">En nuestras tiendas vaz a encontrar las mejores guitarras Acusticas y al mejor precio del mercado, ya que usamos los mejores 
                            materiales y elementos a la hora de la creacion de nuestras guitarras. Nuestros productos son reconocidos internacionalemente y utilizados
                            por muchos famosos musicos y productores.</p>
                                    <div class="botonTiposGuitarra">
                                        <button type="button" class="btn btn-danger" >Comprar</button>
                                    </div>
                        </div>
                    </div>
                </div>
                <div class="col-sm-6 col-xs-12 col-lg-4 mt-5">
                        <div class="card">
                                <div class="d-flex justify-content-center p-2">
                                    <img src="../assets/GuitarraElectrica.png" alt="" width="100%" height="700px" style="border-radius: 10px;">
                                </div>
                                <div class="card-body">
                                    <h2 class="tiposGuitarraTitulos">
                                    Guitarras Electricas
                                    </h2>
                                    <p class="card-text">Se toda una estrella del Rock conj nuestras guitarras Electricas y al mejor precio del mercado, ya que usamos los mejores 
                                    materiales y elementos a la hora de la creacion de nuestras guitarras. Nuestros productos son reconocidos internacionalemente y utilizados
                                    por muchos famosos musicos y productores.</p>
                                    <div class="botonTiposGuitarra">
                                        <button type="button" class="btn btn-danger" >Comprar</button>
                                    </div>
                                    
                                </div>
                        </div>
                </div>
            </div>
        </div>
</template>

<script>
    export default {
        name: "ServicesSection",
        
    }
</script>

<style  scoped>
.card-text{
    padding: 10px;
    text-align: justify;
    bottom: 0;
    color:black;
}
.tiposGuitarraTitulos{
    text-align: center;
}
.botonTiposGuitarra {
    display: flex;
    align-items: center;
    justify-content: center;
}
</style>