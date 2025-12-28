<script setup>
import { ref } from 'vue';

const isMobileMenuOpen = ref(false);

const toggleMenu = () => {
  isMobileMenuOpen.value = !isMobileMenuOpen.value;
};
</script>

<template>
  <nav class="navbar" :class="{ 'scrolled': false }">
    <div class="container">
      <div class="navbar-inner">
        <!-- Logo -->
        <div class="logo">
          <img src="/atlasLogo3.png" alt="Atlas Veteriner Kliniği" class="logo-img">
        </div>

        <!-- Desktop Menu -->
        <div class="desktop-menu">
          <a href="#home" class="nav-link">Anasayfa</a>
          <a href="#services" class="nav-link">Hizmetler</a>
          <a href="#about" class="nav-link">Hakkımızda</a>
          <!-- <a href="#team" class="nav-link">Ekibimiz</a> -->
          <a href="#contact" class="nav-link">İletişim</a>
        </div>

        <!-- CTA Button -->
        <div class="cta-container">
          <a href="#contact" class="btn btn-dark">Randevu Al</a>
        </div>

        <!-- Mobile Menu Button -->
        <div class="mobile-toggle">
          <button @click="toggleMenu" class="toggle-btn">
            <i class="fa-solid" :class="isMobileMenuOpen ? 'fa-xmark' : 'fa-bars'"></i>
          </button>
        </div>
      </div>
    </div>

    <!-- Mobile Menu -->
    <div class="mobile-menu" v-if="isMobileMenuOpen">
      <a href="#home" class="mobile-link" @click="toggleMenu">Anasayfa</a>
      <a href="#services" class="mobile-link" @click="toggleMenu">Hizmetler</a>
      <a href="#about" class="mobile-link" @click="toggleMenu">Hakkımızda</a>
      <!-- <a href="#team" class="mobile-link" @click="toggleMenu">Ekibimiz</a> -->
      <a href="#contact" class="mobile-link" @click="toggleMenu">İletişim</a>
      <div class="mobile-cta">
        <a href="#contact" class="btn btn-dark full-width" @click="toggleMenu">Randevu Al</a>
      </div>
    </div>
  </nav>
</template>

<style scoped>
.navbar {
  position: fixed;
  top: 0;
  left: 0;
  width: 100%;
  z-index: 1000;
  background-color: rgba(255, 251, 246, 0.9);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid var(--paw-border);
  transition: all 0.3s ease;
}

.navbar-inner {
  display: flex;
  justify-content: space-between;
  align-items: center;
  height: 80px;
}

/* Logo */
.logo {
  display: flex;
  align-items: center;
  cursor: pointer;
}

.logo-img {
  height: 50px;
  width: auto;
  object-fit: contain;
}

/* Desktop Menu */
.desktop-menu {
  display: none;
  gap: 2rem;
  align-items: center;
}

.nav-link {
  font-weight: 600;
  color: var(--paw-dark);
  position: relative;
  transition: color 0.3s;
}

.nav-link:hover {
  color: var(--paw-orange);
}

.nav-link::after {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  bottom: -4px;
  left: 0;
  background-color: var(--paw-orange);
  transition: width 0.3s;
}

.nav-link:hover::after {
  width: 100%;
}

/* CTA */
.cta-container {
  display: none;
}

/* Mobile Toggle */
.mobile-toggle {
  display: flex;
  align-items: center;
}

.toggle-btn {
  background: none;
  border: none;
  font-size: 1.5rem;
  color: var(--paw-dark);
  cursor: pointer;
}

/* Mobile Menu */
.mobile-menu {
  position: absolute;
  top: 80px;
  left: 0;
  width: 100%;
  background-color: var(--paw-bg);
  border-bottom: 1px solid var(--paw-border);
  padding: 1rem;
  display: flex;
  flex-direction: column;
  gap: 1rem;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
}

.mobile-link {
  font-weight: 600;
  color: var(--paw-dark);
  padding: 0.5rem 0;
}

.full-width {
  width: 100%;
}

@media (min-width: 768px) {
  .desktop-menu {
    display: flex;
  }
  .cta-container {
    display: flex;
  }
  .mobile-toggle {
    display: none;
  }
  .mobile-menu {
    display: none;
  }
}
</style>
