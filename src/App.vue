<template>
  <div id="app">
    <nav>
      <ImageText/>
    </nav>
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
    <div class="container-fluid" id="team">
      <div class="bordeEquipo">
        <h2 class="estitloTiulo">EQUIPO 41</h2>
      </div>
        <div class="row justify-content-center mb-5">
          <div class="col mt-5" v-for="(miembro, index) of Team" :key="index">
            <TeamCard :member="miembro"></TeamCard>
        </div>    
      </div>
    </div>
    <footer>
      <FooterSection/>
    </footer>
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
          
  "Team": [
    {
      "codigo": "001",
      "nombre": "Miguel Urquijo",
      "descripcion": `Miguel Urquijo nacio en Medellin Colombia y trabaja en Selina en el equipo de tecnologia. Tiene conocimiento previos en ciencias 
      de datos, Machine Learning, Salesforce SDX. Lorem ipsom Lorem Ipsum Lorem ipsom Lorem Ipsum`,
      "rol": "Desarrollador Web",
      "image": "https://i.ibb.co/nQ3Hkbc/Miguel.jpg"
    },
        {
      "codigo": "002",
      "nombre": "David Castaño",
      "descripcion": `David es un empresario colombiano, creador junto con Didier Amaya de MisionTIC. Se la consideraba la décima persona más 
      rica del mundo en el 2019 con una fortuna alrededor de los 54,7 miles de millones de dólares Americanos.`,
      "rol": "Desarrollador Web",
      "image": "https://i.ibb.co/12446FD/david.jpg"
    },
        {
      "codigo": "003",
      "nombre": "Didier Amaya",
      "descripcion": `Didier es un empresario e informático teórico colombiano de origen ruso que, junto a David, fundó Guitarras DavidFender. 
      En conjunto, David y Didier aún mantienen el control de un 16% de la compañía y hacen parte del grupo 41.`,
      "rol": "Desarrollador Web",
      "image": "https://i.ibb.co/ggJsBZP/Didier.jpg"
    },
        {
      "codigo": "004",
      "nombre": "Johamn Albarracin",
      "descripcion": `Es un empresario y magnate colombiano. Es el fundador y director ejecutivo de Guitarras DavidFender. En 2015 fue el quinto 
      hombre más rico del mundo, y en 2017 alcanzó el primer puesto de la lista Forbes.`,
      "rol": "Desarrollador Web",
      "image": "https://i.ibb.co/59rZwXJ/Jhoam.jpg"
    }
    ]
}    
}

           }
    

</script>


<style  scoped>
.bordeEquipo{
    border-style: solid;
    border-width: 0px 0px 2px 0px;
    margin-right: 60px;
    margin-left: 60px;
    border-color:black;
    text-align: center;
    padding-top: 15px;

}

.estitloTiulo {
  align: center;

}

.borde{
    border-style: solid;
    border-width: 2px 0px 0px 0px;
    margin-right: 60px;
    margin-left: 60px;
    border-color:black;

}
</style>



