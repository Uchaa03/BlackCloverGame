<template>
  <section class="video-section py-5">
    <div class="container">
      <h2 class="text-center mb-4 fw-bold">Trailer del Juego</h2>

      <div class="row">
        <article class="col-12">
          <figure class="position-relative mb-4">
            <!-- video con múltiples formatos convertidos con ffmpeg -->
            <video
                class="w-100 shadow"
                controls
                preload="metadata"
                poster="@/assets/img/Miniatura.png">
              <source src="@/assets/video/trailer.webm" type="video/webm">
              <source src="@/assets/video/trailer.mp4" type="video/mp4">
              <p class="fallback-text">Tu navegador no soporta video HTML5.</p>
            </video>
            <figcaption class="text-center text-muted mt-2">
              Explora el mundo de Black Clover en formato pixel art
            </figcaption>
          </figure>

          <!-- También e puesto un audio para añadir mas formatos -->
          <section class="audio-section mt-5">
            <h3 class="h5 text-center mb-3">Banda Sonora</h3>
            <div class="d-flex justify-content-center">
              <audio class="w-75" controls preload="none">
                <source src="@/assets/audio/theme.mp3" type="audio/mpeg">
                <source src="@/assets/audio/theme.ogg" type="audio/ogg">
              </audio>
            </div>
            <p class="text-center text-muted small mt-2">
              Música: "Haruka Mirai" - Tema oficial de Black Clover
            </p>
          </section>
        </article>
      </div>
    </div>
  </section>
</template>


<script>
  export default {
    name: "SectionVideoComponent"
  }
</script>

<style scoped>
  .video-section {
    background-color: #f5f5f5;
  }

  video {
    max-height: 600px;
    background-color: #000;
  }

  audio {
    border-radius: 30px;
    box-shadow: 0 4px 6px rgba(0,0,0,0.1);
  }

  @media (max-width: 768px) {
    video {
      max-height: 300px;
    }

    audio {
      width: 100% !important;
    }
  }
</style>
