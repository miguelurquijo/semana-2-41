<template>
    <div>
        <div class="card text-black">
            <div class="d-flex justify-content-center p-2">
                <img :src="member.image" alt="Foto del Equipo" height="200px" class="EstiloImagen">
            </div>
            <div class="card-body">
                <p class="card-text">Codigo: {{member.codigo}}</p>
                    <h5 class="card-title">{{member.nombre}}</h5>
                    <p class="card-text">{{member.descripcion}}</p>
                    <p class="card-text">{{member.rol}}</p>
                </div>
            </div>
        </div> 
</template>

<script>
    export default {
        name: "TeamCard",
        props: ['member']
    }
</script>

<style scoped>
    .EstiloImagen {
        border-radius: 10px;
        object-fit: cover;
        width: 100%;
        height: 250PX;
    }

    .borde{
        border-style: solid;
        border-width: 2px 0px 0px 0px;
        margin-right: 60px;
        margin-left: 60px;
        border-color:black;
        outline: 0;
}

.card:hover {
    border: 1px solid;
    padding: 10px;
    box-shadow: 0 2px 1px rgba(0,0,0,0.5);
    transition: opacity 0.3s ease-in-out;
    outline: 0;
  
}
</style>
