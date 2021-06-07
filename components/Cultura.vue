<template>

  <section class="seccion_1">
    

    <div data-aos="zoom-in" data-aos-duration="2000">
      <img class="img_estilos" src="../static/Cultura.png" alt />
    </div>


    <br>
    <br>
    
    <h1 data-aos="fade-up" data-aos-easing="ease"  data-aos-duration="1000" class="secciones">Cultura</h1>
    
    <br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">1</span>Templo de Kiyomizu-dera (Kioto)</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Situado en una colina con vistas al valle y a la ciudad, 
      Kiyomizu-dera es el templo más visitado de Kioto. Fue construido en honor a Kannon, la diosa de la
       misericordia. A menudo, se celebran en este templo eventos peculiares, a parte de las celebraciones 
       cotidianas del recinto, como la noche en que se ilumina el templo en color rosa para concienciar 
       sobre el cáncer de mama o las producciones teatrales.
    </p><br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">2</span>Templo Kinkakuji (Kioto)</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Kinkakuji fue construido originalmente en 1397 como el hogar de 
      un shogun o un jefe militar. El edificio estaba cubierto completamente con pan de oro, dándole el título de 
      Pabellón Dorado. Sus jardines están destinados a representar un paraíso terrenal.
    </p><br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">3</span>Templo Senso-ji (Tokio)</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Según la leyenda, dos hermanos intentaron repetidamente devolver una
      estatua de la diosa Kannon al río Sumida. Cada vez que lo hacían, la estatua regresaba al templo al día siguiente. 
      El templo Senso-ji fue construido en ese lugar en honor a la diosa. Su belleza es mayor por la noche cuando la iluminación nocturna resalta su compleja arquitectura.
    </p><br>
 
    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">4</span>Templo de Hokokuji (Kamakura)</h2>
    <p data-aos="fade-up" data-aos-duration="2000">También llamado el Templo de Takedera, sus jardines albergan bosques de bambú, 
      delicadas esculturas cubiertas de musgo y estanques de koi de colores brillantes. Hasta las 3 p.m. 
      puedes disfrutar de un auténtico matcha japonés (té verde molido) con dulces en las instalaciones del templo.
    </p><br>

    <img class="logo" src="../static/logo_flor.png" />

  
  </section>
  
  
  
  
</template>







<script>
  export default {
    
  }
</script>


<style>

.circulo{
  background: #f39e9c;
  border-radius: 0.8em;
  color: #fff;
  display: inline-block;
  font-weight: bold;
  line-height: 1.6em;
  margin-right: 15px;
  text-align: center;
  width: 1.6em; 
  margin-left: -2.5rem;
}

.img_estilos{
  margin-left: 22.5rem;
  position: relative;
  max-width: 50rem;
}

.secciones{
  margin-left: 22.5rem;
  color: #33355d;
  font-size: 3rem;
}

h2{
  margin-left: 26rem;
  color: #67729b;
}

.before-enter{
  opacity: 0;
  transform: translateY(100px);
  transition: all 2s ease-out;

}

.enter{
  opacity: 1;
  transform: translateY(0px);
  
}

.logo{
  margin-left: 42rem;
  margin-top: 5rem;

  
}




</style>
