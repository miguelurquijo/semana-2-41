<template>
  <div id="app">
    <ImageText/>
    <CarouselSection/>
    <ServicesSection/>
    <!--News-->

        <div class="container-fluid"> 
              <div class="d-flex justify-content-center align-items-center" >
                <h2 class="tituloNoticias">Seccion de Noticias</h2>
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



