<template>
<div>
  <Nav></Nav>
<div class="projets"> 
<!--<img alt="Vue logo" src="../assets/image1.png">-->
<HelloWorld msg="Welcome to Your Vue.js App"/>

<div class="card-group">
  <div class="card">
    <img src="../assets/Plume.jpg" class="card-img-top" alt="...">
    <div class="card-body">
      <h3 class="card-title">Écriture(Nouvelles)</h3>
      <p class="card-text">Dépuis 2016, j'écris des nouvelles, courtes et faciles à lire normalement :-). </p>
      <p>  <router-link to="/projects/ecriture"><b-button variant="primary">Suivre</b-button></router-link></p>
      
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated 3 mins ago</small>
    </div>
  </div>

  <div class="card">
    <img src="../assets/pl.png" class="card-img-top" alt="https://www.barinta.org">
    <div class="card-body">
      <h3 class="card-title">Association Barinta</h3>
      <p class="card-text">Barinta est une association fondée en 2017 par <a href="https://www.linkedin.com/in/cheick-mahady-sissoko-45482b63/">Cheick Mahady Sissoko </a> 
      et moi même.<br> Ella a pour objetif de soutenir l'éducation des enfants dans les zones défavorisées de l'Afrique de l'Ouest.<br>
      <router-link to="/projects/barinta"><b-button variant="primary">En savoir plus</b-button></router-link>
     </p>
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated 3 mins ago</small>
    </div>
  </div>

  <div class="card">
    <img src="../assets/innovafrq.jpg" class="card-img-top" alt="...">
    <div class="card-body">
      <h3 class="card-title">Plan d'Action Pour l'Afrique</h3>
      <p class="card-text">L'Afrique est probablement le continent le plus riche en terme de matières premières dans le monde.<br>Alors pourquoi est-elle la plus sous-développée?<br>Qu'avons-nous à apporter en tant que jeunes?</p>
      <p><router-link to="/projects/paa"><b-button variant="primary">En savoir plus</b-button></router-link></p>
    </div>
    <div class="card-footer">
      <small class="text-muted">Last updated 3 mins ago</small>
    </div>
  </div>


</div>
</div>
</div>
</template>

<script>
import Nav from '@/components/Nav.vue'
export default {
name:'projets',
components: 
{
Nav,  
}
}
</script>

<style> </style>