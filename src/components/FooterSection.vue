<template>
        <!-- Footer -->
    <footer class="page-footer bg-secondary text-white pt-4">
    
        <!-- Footer Text -->
        <div class="container-fluid text-center text-md-left">
    
            <!-- Grid row -->
            <div class="row">
    
                <!-- Grid column -->
                <div class="col-md-6 mt-md-0 mt-3">
    
                    <!-- Content -->
                    <p>Repositorio del proyecto</p>
                    <p>Creador: Grupo 41</p>
                    <p>Contacto: grupo41@misiontic.com</p>
    
                </div>
                <!-- Grid column -->
    
                <hr class="clearfix w-100 d-md-none pb-3">
    
                <!-- Grid column -->
                <div class="col-md-6 mb-md-0 mb-3">
    
                    <!-- Content -->
                    <ui>
                        <li><a class="estilosVinvulos" href="https://www.w3schools.com/"  target="_blank">Politica de privacidad</a></li>
                        <li><a class="estilosVinvulos" href="https://www.w3schools.com/"  target="_blank">Condiciones de uso</a></li>
                        <li><a class="estilosVinvulos" href="https://www.w3schools.com/"  target="_blank">Declaracion de accesibilidad</a></li>
                    </ui>
    
                </div>
                <!-- Grid column -->
    
            </div>
            <!-- Grid row -->
    
        </div>
        <!-- Footer Text -->
    
        <!-- Copyright -->
        <div class="footer-copyright text-center py-1 bg-">Copyright ©2020. DavidFender Musical Instruments Corporation. All Rights Reserved.
        </div>
        <!-- Copyright -->
    
    </footer>
</template>
<style>

.estilosVinvulos {
    color: white;
}

.estilosVinvulos:link {
  text-decoration: none;
}

.estilosVinvulos:visited {
  text-decoration: none;
}

.estilosVinvulos:hover {
  text-decoration: underline;
}

.estilosVinvulos:active {
  text-decoration: underline;
}
</style>
<script>
    export default {
        name: "FooterSection",
        
    }
</script>