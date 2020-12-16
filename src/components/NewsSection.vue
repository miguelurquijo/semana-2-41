<template>          
            <div class="row mt-md-5 mt-sm-5 mt-xs-5">
                
                <div id="news-container" class="col-lg-6 col-xs-12" v-for="(noticia, index) of noticias" :key = index>
                    <div id="news-data" class="d-flex justify-content-center align-items-center">
                        
                        <div class="p-3">
                            <img class="imagenNews" :src="noticia.image" alt="" width="350em" height="300em" style="border-radius: 10px">
                        </div>
        
                        <div class="p-2">
                            <h4>{{noticia.title}}</h4>
                            <p>
                                {{noticia.description}}
                            </p>
                        </div>       
                    </div>
                    <div id="news-url" class="d-flex container-fluid justify-content-end pb-2 mt-n2">
                        <button  type="button" @click="triggerClick(noticia.url)" target="" class="btn btn-danger" >Pagina News</button>
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
                noticias: null
            }
            
        },
        created(){
            axios
                .get('https://gnews.io/api/v4/top-headlines?&token=d6db0420dc11cc2f84a13823b774edc1&max=10')
                .then(response => { this.noticias = response.data.articles.slice(0,4) })
        },
              methods:{
        triggerClick: function (number){
            window.open(number,'_blank');
        }

      }
    }
</script>

<style scoped>

</style>