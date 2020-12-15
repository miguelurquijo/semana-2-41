<template>          
            <div class="row mt-md-5 mt-sm-5 mt-xs-5">
                
                <div class="col-lg-6 col-xs-12" v-for="(pelicula, index) of peliculas" :key = index>
                    <div class="d-flex justify-content-center align-items-center">
                        
                        <div class="p-3">
                            <img class="imagenNews" :src="pelicula.image" alt="" width="300em" height="300em" style="border-radius: 10px">
                        </div>
        
                        <div class="p-2">
                            <h4>{{pelicula.title}}</h4>
                            <h6>{{pelicula.description}}</h6>
                            <p>
                                Lorem, ipsum dolor sit amet consectetur adipisicing elit. Ut ratione harum voluptates nulla laudantium! Aut, 
                                possimus. Expedita unde maiores reprehenderit, quibusdam blanditiis beatae doloremque? Corporis laudantium veritatis omnis accusantium error.
                            </p>
                        </div>
        
                    </div>
                    <div class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                        <button  type="button" @click="pelicula.url" target="_blank" class="btn btn-outline-info"> Info</button>
                    </div>
                </div>
           </div>
</template>


<script>
import axios from "axios"

    export default {
        name: "NewsSection",
        data(){
            return{
                peliculas: null
            }
            
        },
        created(){
            axios
                .get('https://gnews.io/api/v4/top-headlines?&token=dbb79ab882316df3fb72b08552a98dc8&max=10')
                .then(response => { this.peliculas = response.data.articles.slice(0,4) })
        }
    }
</script>

<style scoped>

</style>