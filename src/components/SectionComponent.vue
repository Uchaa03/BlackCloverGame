<template>
  <section class="row g-4">
    <!-- Sección de descripción -->
    <article class="col-md-6 d-flex flex-column justify-content-start">
      <h2 class="mb-4 fw-bold mt-0">Concepto Pixel Art</h2>
      <p class="lead">Black Clover Game recrea el universo mágico medieval en un estilo retro de pixel art,
        combinando la rica narrativa del anime con mecánicas clásicas de plataformas.</p>
      <p>El diseño en pixel art permite capturar la esencia de los personajes mientras ofrece una experiencia
        nostálgica que rinde homenaje a los juegos clásicos. Cada elemento ha sido cuidadosamente diseñado para
        mantener la personalidad única de la serie original.</p>
      <p>Los escenarios, desde la aldea Hage hasta el castillo de los Caballeros Mágicos, son recreados
        con detallados sprites que evocan la atmósfera mágica del mundo de Black Clover.</p>
    </article>

    <!-- Tarjeta con animación al hacer click -->
    <article class="col-md-6 d-flex justify-content-lg-end justify-content-center align-items-start">
      <figure
          class="flip-card"
          @click="toggleFlip"

          :class="{ 'is-flipped': isFlipped }">     <!-- Flag básica para cambiar la clase -->
        <div class="flip-card-inner">
          <!-- Parte delantera -->
          <section class="flip-card-front bg-light border rounded p-3 d-flex flex-column align-items-center shadow">
            <h3 class="card-title mb-3">Asta - Personaje Principal</h3>
            <img src="@/assets/img/AstaPersonaje.png" alt="Asta Pixel Art" class="img-fluid mb-3">
            <p class="text-center text-muted small">¡Haz clic para descubrir más!</p>
          </section>
          <!-- Parte trasera -->
          <section class="flip-card-back bg-dark text-light border rounded p-4 shadow">
            <h3 class="card-title mb-3">Asta</h3>
            <p>Joven huérfano sin poderes mágicos en un mundo donde la magia lo es todo. A pesar de esta
              desventaja, Asta posee una determinación inquebrantable.</p>
            <p>Su grimorio de cinco hojas contiene una misteriosa espada anti-magia que le permite anular
              cualquier hechizo, ya que lleva un demonio dentro *liebe*.</p>
            <p class="fst-italic">"¡Mi magia es no rendirme!"</p>
          </section>
        </div>
      </figure>
    </article>
  </section>
</template>

<script>
export default {
  name: "SectionComponent",
  data() {
    return {
      isFlipped: false
    }
  },
  methods: {
    toggleFlip() {
      this.isFlipped = !this.isFlipped;
    }
  }
}
</script>

<style scoped>
  .flip-card {
    width: 400px;
    height: 500px;
    perspective: 1000px;
    cursor: pointer;
    margin: 0;
  }

  .flip-card-inner {
    position: relative;
    width: 100%;
    height: 100%;
    transition: transform 0.8s;
    transform-style: preserve-3d;
  }

  .flip-card.is-flipped .flip-card-inner {
    transform: rotateY(180deg);
  }

  .flip-card-front, .flip-card-back {
    position: absolute;
    width: 100%;
    height: 100%;
    -webkit-backface-visibility: hidden;
    backface-visibility: hidden;
    overflow: hidden;
  }

  .flip-card-back {
    transform: rotateY(180deg);
  }
</style>
