<template>
  <Bannier />
  <NosOffres />
  <CalculateBMI />
  <NosClasses />
  <EquipmentsPage />
  <NosFormateurs />
  <ContactUS />
  <FooterPage />
</template>

<script>
import Bannier from './components/banier/bannier.vue'
import NosClasses from './components/nos_offre/NosClasses.vue'
import EquipmentsPage from './components/nos_offre/Equipments.vue'
import CalculateBMI from './components/nos_offre/CalculateBMI.vue'
import NosFormateurs from './components/nos_offre/NosFormateurs.vue'
import NosOffres from './components/nos_offre/NosOffres.vue'
import ContactUS from './components/nos_offre/ContactUS.vue'
import FooterPage from './components/nos_offre/Footer.vue'

export default {
  name: 'App',
  components: {
    Bannier,
    NosOffres,
    NosClasses,
    EquipmentsPage,
    CalculateBMI,
    NosFormateurs,
    ContactUS,
    FooterPage,
  }
}
</script>

<style>
#app {
  font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  /* margin-top: 60px; */
}
</style>
