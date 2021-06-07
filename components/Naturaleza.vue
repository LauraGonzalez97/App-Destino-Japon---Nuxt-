<template>

  <section class="seccion_1">
    

    <div data-aos="zoom-in" data-aos-duration="2000">
      <img class="img_estilos" src="../static/Naturaleza.png" alt />
    </div>


    <br>
    <br>
    
    <h1 data-aos="fade-up" data-aos-easing="ease"  data-aos-duration="1000" class="secciones">Naturaleza</h1>
    
    <br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">1</span>Bosque Nara</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Poner un pie en la ciudad de Nara es adentrarse en el Japón más tradicional.
    Bien es cierto que en un primer momento lo que más llama la atención al visitar Nara es la dominante presencia
    de unos seres de cuatro patas, cuernos y apetito voraz. Los ciervos son los amos y señores de gran parte de 
    Nara no en vano hacen guardia a lo largo y ancho del parque donde se localizan la gran mayoría de los 
    templos de la ciudad de Nara.
    </p><br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">2</span>Bosque Kasugayama</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Localizado justo detrás del Santuario Kasuga Taisha se trata de un bosque 
    primitivo que alberga una gran variedad animal y vegetal. Su estado de conservación es tan  bueno que este 
    bosque da una imagen clara de como eran los bosques primitivos en esta parte de Japón, no en vano en 1924 se 
    declaro monumento nacional del país y el 1955 obtuvo una distinción como monumento natural especialmente 
    protegido lo cual ha impedido actividades como la caza o la construcción en su interior.
    </p><br>

    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">3</span>Parque Nacional de Shiretoko</h2>
    <p data-aos="fade-up" data-aos-duration="2000">Este parque del norte de la isla de Hokkaido está considerado Patrimonio Universal 
    de la Humanidad por la UNESCO. Uno de los aspectos más destacados de este parque es la gran población de osos pardos. 
    Durante los meses de verano, observar a los osos desde los barcos turísticos es una actividad muy  popular. 
    Y en el invierno, hielo cubre las carreteras, y atravesar el parque queda reservado exclusivamente a los
     aventureros, que pueden hacerlo en barco o a pie.
    </p><br>
 
    <h2 data-aos="fade-right" data-aos-duration="1000"><span class="circulo">4</span>Parque Nacional de Fuji Hakone Izu</h2>
    <p data-aos="fade-up" data-aos-duration="2000">El de Fuji es, sin duda, el parque nacional más popular de Japón. El majestuoso e 
    icónico Monte Fuji, un volcán activo, ofrece actividades muy variadas que van desde la escalada en la montaña 
    hasta tomar el sol en las playas de arena, o relajarse en un onsen.
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
