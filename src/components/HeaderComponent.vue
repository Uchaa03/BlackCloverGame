<template>
  <header>
    <section class="container py-2">
      <article class="row align-items-center">
        <figure class="col-3 col-sm-2 col-md-1 mb-0">
          <img src="@/assets/img/Logo.png" alt="Logo" class="img-fluid">
        </figure>

        <section class="col-9 col-sm-10 col-md-11">
          <h1 class="text-end fw-bold mb-0">BLACK CLOVER GAME</h1>
        </section>
      </article>
    </section>
  </header>
</template>

<script>
  export default {
    name: "HeaderComponent"
  }
</script>

<style scoped>
  header {
    box-shadow: 0 4px 8px 0 rgba(0, 0, 0, 0.2), 0 6px 20px 0 rgba(0, 0, 0, 0.19);
  }
</style>