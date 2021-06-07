<template>

  <section class="seccion_1">
    

    <div data-aos="zoom-in" data-aos-duration="2000">
      <img class="img_estilos" src="../static/gastronomia.png" alt />
    </div>


    <br>
    <br>
    
    <h1 data-aos="fade-up" data-aos-easing="ease"  data-aos-duration="1000" class="secciones">Gastronomía</h1>
    
    <br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">1</span>Kitakata Ramen Bannai</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Es una cadena de restaurantes especializados en ramen de Kitakata, 
      uno de los tres ramen más famosos de Japón junto con el de Sapporo y 
      el de Hakata. Su local original se encuentra en Kitakata (Fukushima), 
      pero tiene locales en Tokio y hasta Kioto y Osaka, entre otras muchas ciudades.
    </p><br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">2</span>Ichiran Ramen</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Es una cadena especializada en tonkotsu ramen con gran presencia en todo el país. 
      ¿Su particularidad? La posibilidad de comer en absoluta privacidad y no tener apenas 
      contacto con nadie. Además de un caldo delicioso, todo sea dicho.
    </p><br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">3</span>Hakkoku</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Es una espectacular barra de sushi en Ginza. 
      En realidad son tres pequeñas barras en un mismo local, con una calidad inmejorable.
    </p><br>
 
    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">4</span>Kobe Beef Kaiseki 511</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Es un restaurante especializado, como su propio nombre indica, en carne de Kobe. 
      Disponen de dos menús centrados en la carne de Kobe (uno occidental, otro japonés) 
      además de poder comer a la carta. En breve os hablaremos de nuestra experiencia allí.
    </p><br>

  
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

</style>
