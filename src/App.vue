<script setup>
import Header from './components/Header.vue'
import HeroSection from './components/HeroSection.vue'
import SectionCard from './components/SectionCard.vue'
import Newbies from './components/Newbies.vue'
import TeamSection from './components/TeamSection.vue'
import CatalogCard from './components/CatalogCard.vue'
import Footer from './components/Footer.vue'
</script>

<template>
  <Header />
  <main>
    <HeroSection />
    <SectionCard />
    <Newbies />
    <TeamSection />
    <CatalogCard />
  </main>
  <Footer />
</template>

<style scoped></style>
