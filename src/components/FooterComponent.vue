<template>
  <footer class="mt-5 py-4 border-top">
    <div class="container">
      <div class="row">
        <section class="col-12 text-center">
          <p xmlns:cc="http://creativecommons.org/ns#"
             xmlns:dct="http://purl.org/dc/terms/">
            <a property="dct:title" rel="cc:attributionURL" href="https://github.com/Uchaa03/BlackCloverGame">BlackCloverGame</a>
            by
            <a rel="cc:attributionURL dct:creator" property="cc:attributionName" href="https://github.com/Uchaa03">Adrián Ucha Sousa</a>
            is licensed under
            <a href="https://creativecommons.org/licenses/by-nc/4.0/?ref=chooser-v1" target="_blank" rel="license noopener noreferrer" style="display:inline-block;">
              CC BY-NC 4.0
              <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/cc.svg?ref=chooser-v1" alt="">
              <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/by.svg?ref=chooser-v1" alt="">
              <img style="height:22px!important;margin-left:3px;vertical-align:text-bottom;" src="https://mirrors.creativecommons.org/presskit/icons/nc.svg?ref=chooser-v1" alt="">
            </a>
          </p>
        </section>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: "FooterComponent"
}
</script>

<style scoped>
  footer {
    background-color: #f8f9fa;
    border-top: 4px solid #ddd;
  }

  footer p {
    font-size: 0.9rem;
    letter-spacing: 0.05em;
  }

  footer small {
    font-size: 0.7rem;
  }
</style>