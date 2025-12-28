<script setup>
import NavBar from './components/NavBar.vue'
import HeroSection from './components/HeroSection.vue'
import ServicesSection from './components/ServicesSection.vue'
import WhyChooseUs from './components/WhyChooseUs.vue'
import TeamSection from './components/TeamSection.vue'
import TestimonialsSection from './components/TestimonialsSection.vue'
import AppointmentSection from './components/AppointmentSection.vue'
import AppFooter from './components/AppFooter.vue'
</script>

<template>
  <NavBar />
  <main>
    <HeroSection />
    <ServicesSection />
    <WhyChooseUs />
    <!-- <TeamSection /> -->
    <!-- <TestimonialsSection /> -->
    <AppointmentSection />
  </main>
  <AppFooter />
</template>

<style>
/* Global styles are in style.css */
</style>
