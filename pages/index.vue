<template>
<div>
  <Nav></Nav>
  <section class="container">
    <div class="header-overlay">
      <logo />
      <h1 class="title">
        Oumou Sow
      </h1>
      <h2 class="subtitle">
       Binvenue
      </h2>
      <div class="links">
        <a
          href="https://nuxtjs.org/"
          target="_blank"
          class="button--green"
        >Documentation</a>
        <a
          href="https://github.com/nuxt/nuxt.js"
          target="_blank"
          class="button--grey"
        >GitHub</a>
      </div>
    </div>
  </section>
  </div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import Nav from '@/components/Nav.vue'
export default {
  components: {
   Logo,
    Nav
  }
}
</script>

<style>
.container {
  margin:0 auto;
  min-height: 0vh;
  display: flex;
  justify-content: center;
  align-items: center;
  text-align: center;
  /*background-image:url("../assets/image1.png");
  background-repeat: no-repeat;
  background-position:100% 100%;
  background-origin:border-box;
  width: 100%;
  height: auto;*/
}
.header-overlay {
  background: rgba(0,0,0,0.4);
  color: white;
  height:670px;
  font-weight: bold;
  font-size: 20px;
  width: 940px;
  padding:0px;
}
.title {
  font-family: 'Quicksand', 'Source Sans Pro', -apple-system, BlinkMacSystemFont,
    'Segoe UI', Roboto, 'Helvetica Neue', Arial, sans-serif;
  display: block;
  font-weight: 300;
  font-size: 100px;
  color: #35495e;
  letter-spacing: 1px;
  padding: 15%;
}

.subtitle {
  font-weight: 300;
  font-size: 42px;
  color: #526488;
  word-spacing: 5px;
  padding-bottom: 15px;
}

.links {
  padding-top: 15px;
}

#fondecran {
 /* Fixe l'image en haut à gauche de la page */
 position: fixed; 
 top: 0; 
 left: 0; 
 /* Préserve le ratio de l'image */
 min-width: 100%;
 min-height: 100%;
}

img.fondecran {
 /* On met en place le fond d'écran */
 min-height: 100%;
 min-width: 1024px;
 /* On indique un redimensionnement proportionnel */
 width: 100%;
 height: auto;
 /* L'image est positionnée en haut à gauche */
 position: fixed;
 top: 0;
 left: 0;
}
@media screen and (max-width: 1024px) { /* Le traitement est ici spécifique à l'image */
 img.fondecran {
 left: 50%;
 margin-left: -512px; /* 50% */
 }
}
</style>
