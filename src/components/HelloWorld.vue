<template>
  <v-carousel
  >
  <v-carousel-item v-for="(img, index) in imagen" :key="index">
      <v-img :src="img.src" :alt="img.alt" cover></v-img>
      <div class="carousel-text">
        <h2>{{ slides[index].title }}</h2>
        <p>{{ slides[index].info }}</p>
      </div>
    </v-carousel-item>
  </v-carousel>
</template>

<script>
  export default {
    data () {
      return {
        imagen: [
        { src: 'https://github.com/giandeveloper2109/PenayFauraWebPage2023/blob/main/src/assets/Imagenes/Carrusel/carrusel1.jpg?raw=true'},
        { src: 'https://github.com/giandeveloper2109/PenayFauraWebPage2023/blob/main/src/assets/Imagenes/Carrusel/carrusel2.jpg?raw=true'},
        { src: 'https://github.com/giandeveloper2109/PenayFauraWebPage2023/blob/main/src/assets/Imagenes/Carrusel/carrusel3.jpg?raw=true'},
        { src: 'https://github.com/giandeveloper2109/PenayFauraWebPage2023/blob/main/src/assets/Imagenes/Carrusel/carrusel4.jpg?raw=true'},
        { src: 'https://github.com/giandeveloper2109/PenayFauraWebPage2023/blob/main/src/assets/Imagenes/Carrusel/carrusel5.jpg?raw=true'},
        { src: 'https://github.com/giandeveloper2109/PenayFauraWebPage2023/blob/main/src/assets/Imagenes/Carrusel/carrusel6.jpg?raw=true'},
        ],
        slides: [
        { title: 'MENSAJE IMPORTANTE:', info: 'Estimados señores, acatando las medidas de urgencia que ha dado el gobierno, queremos hacer de su conocimiento que nuestro Despacho continuará brindándoles el soporte y asesoría legal que ustedes puedan requerir, para lo cual les recordamos que nuestros correos electrónicos, celulares, mensajes de texto y Whatsapp, se mantienen a su entera disposición. No duden en llamar a nuestra central telefónica para canalizar sus consultas con el especialista que requiera.' },
        { title: 'Asesoría y consultoría', info: 'Somos una organización conformada por profesionales expertos en sus diversas especialidades. Prestamos servicios de asesoría y consultoría a importantes clientes que operan en un variado campo de actividades, tales como servicios, industrias, comercio, minería y construcción entre otras.' },
        { title: 'Conocimientos y Experiencias', info: 'Los socios y nuestros consultores comparten sus conocimientos y experiencias, de manera que en cada compromiso se tiene disponible el apoyo ilimitado de profesionales especializados en sus diversas disciplinas de la práctica profesional.' },
        { title: 'Comunidad de Interés', info: 'Nuestra forma de organización genera los beneficios que se derivan de una comunidad de interés, uniformidad y control de calidad de nuestra práctica en todo el medio, recibiendo nuestros clientes la misma calidad del servicio profesional, independientemente del lugar de sus operaciones.' },
        { title: 'Experiencia y Contactos', info: 'El principal recurso de nuestra firma es nuestra experiencia y contactos a nivel nacional e internacional sobre la que no escatimamos esfuerzos para que continúe en crecimiento y actualización constante.' },
        { title: 'Técnicas y Conocimientos', info: 'Nuestra política de cooperación en el desarrollo de la actividad empresarial en el país, el constante esfuerzo para mantenernos actualizados en técnicas y conocimientos a nivel internacional, el cumplimiento de una estricta ética profesional y nuestras elevadas normas de calidad y rendimiento en el trabajo, han permitido que accionistas, inversionistas y usuarios, aprovechen los servicios que les brindamos con plena confianza y seguridad.' },
      ],
      }
    },
  }
</script>
<style scoped> 
.carousel-text {
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  transform: translateY(-50%);
  color: white;
  padding: 10px;
  text-align: center;
}
.carousel-text h2 {
  margin: 0;
  font-size: 30px;
  color: rgb(249, 50, 50);
}

.carousel-text p {
  margin: 10px 0 0;
  font-size: 18px;
  max-width: 500px; 
  margin-left: auto;
  margin-right: auto;
  color: rgb(0, 0, 0);
}
</style>