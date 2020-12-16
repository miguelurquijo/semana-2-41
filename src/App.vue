<template>
  <div id="app">
    <ImageText/>
    <CarouselSection/>
    <br>
      <div id="services" class="container-fluid">
        <div class="d-flex justify-content-center align-items-center" >
            <h2 class="tituloNoticias">TIPOS DE GUITARRAS</h2>
          </div> 
          <div class="borde">
          </div>
          <ServicesSection/>
      </div>    
    <!--News-->

        <div id="news" class="container-fluid"> 
              <div class="d-flex justify-content-center align-items-center" >
                <h2 class="tituloNoticias">SECCION DE NOTICIAS</h2>
              </div>  
              <div class="borde">
              </div>
                     
              <NewsSection></NewsSection>         
        </div>
    <!--Team-->
    <div class="container-fluid">
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(miembro, index) of Team" :key="index">
            <TeamCard :member="miembro"></TeamCard>
          </div>
            
        </div>
    </div>
    <FooterSection/>
  </div>
</template>

<script>

import ImageText from './components/ImageText.vue'
import CarouselSection from './components/CarouselSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import FooterSection from './components/FooterSection.vue'
import TeamCard from './components/TeamCard.vue'
import NewsSection from './components/NewsSection.vue'

export default {
  name: 'App',
  components:{
    ImageText,
    CarouselSection,
    ServicesSection,
    FooterSection,
    TeamCard,
    NewsSection
  },
  data(){
    return{
      // aqui va el listado del equipo en forma de JSON
    }
  }
}
</script>

<style  scoped>
.borde{
    border-style: solid;
    border-width: 2px 0px 0px 0px;
    margin-right: 60px;
    margin-left: 60px;
    border-color:black;
}
</style>



