<template>
  <section class="platform-section py-5">
    <div class="container">
      <div class="row g-4">
        <!-- Aqui he puesto la imagen con el art direction aunque la imagen no sea la mejor la funcionalidad la cumple -->
        <figure class="col-lg-6 mb-4 mb-lg-0">
          <picture>
            <!-- Versión móvil -->
            <source
                media="(max-width: 576px)"
                srcset="@/assets/img/Fondobase2.png"
                width="100%">

            <!-- Versión tablet  -->
            <source
                media="(max-width: 992px)"
                srcset="@/assets/img/Fondobase1.png"
                width="100%">

            <!-- Imagen completa para desktop -->
            <img
                src="@/assets/img/Fondobase.png"
                alt="Escenario de plataformas en pixel art"
                class="img-fluid shadow-sm platform-img"
                loading="lazy">
          </picture>
          <figcaption class="text-center text-muted mt-2">Escenario típico de nuestro juego de plataformas</figcaption>
        </figure>

        <!-- Parte del texto de la carta -->
        <article class="col-lg-6">
          <div class="h-100 d-flex flex-column justify-content-center text-end">
            <h2 class="mb-4 fw-bold">Juego de Plataformas</h2>
            <p class="lead">Los juegos de plataformas son experiencias donde el jugador controla un personaje que debe saltar entre superficies suspendidas (plataformas) mientras evita obstáculos.</p>
            <p>En <strong>Black Clover Game</strong>, hemos adaptado esta mecánica clásica para permitir a los jugadores explorar el reino del trébol a través de niveles repletos de desafíos, enemigos y secretos por descubrir.</p>
            <p>El sistema de combate combina saltos precisos con el uso de las habilidades únicas de Asta, creando una experiencia que respeta las raíces del género mientras introduce elementos innovadores de la serie.</p>
          </div>
        </article>
      </div>
    </div>
  </section>
</template>

<script>
  export default {
    name: "Section2Component",
  }
</script>

<style scoped>
  .platform-section {
    position: relative;
    overflow: hidden;
  }

  .platform-img {
    height: auto;
    width: 100%;
  }

  @media (max-width: 992px) {
    .platform-section {
      padding: 3rem 0;
    }
  }
</style>
