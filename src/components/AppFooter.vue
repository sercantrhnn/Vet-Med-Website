<template>
  <footer class="app-footer">
    <div class="container">
      <div class="footer-grid">
        <!-- Brand -->
        <div class="brand-col">
          <div class="brand-logo">
            <img src="/atlasLogo3.png" alt="Atlas Veteriner Kliniği" class="logo-img">
          </div>
          <p class="brand-desc">
            Sevimli dostlarınız için en iyi veteriner hizmetlerini sunuyoruz. Sevgiyle profesyonel bakım.
          </p>
          <div class="social-links">
            <!-- <a href="#" class="social-link"><i class="fa-brands fa-facebook-f"></i></a> -->
            <a href="https://www.instagram.com/atlasveterinertokat/" target="_blank" class="social-link"><i class="fa-brands fa-instagram"></i></a>
            <!-- <a href="#" class="social-link"><i class="fa-brands fa-twitter"></i></a> -->
          </div>
        </div>

        <!-- Links -->
        <div class="links-col">
          <h4 class="footer-title">Hızlı Bağlantılar</h4>
          <ul class="footer-links">
            <li><a href="#home">Anasayfa</a></li>
            <li><a href="#about">Hakkımızda</a></li>
            <li><a href="#services">Hizmetler</a></li>
            <li><a href="#contact">İletişim</a></li>
          </ul>
        </div>

        <!-- Location 1 -->
        <div class="location-col">
          <h4 class="footer-title">Tokat Merkez</h4>
          <ul class="info-list">
            <li>
              <i class="fa-solid fa-location-dot icon"></i>
              <a href="https://maps.app.goo.gl/ZN5ZJ8fQHK7iu5af8" target="_blank" class="hover:text-orange">Altıyüzevler Mah. Vali Ayhan Çevik Cd. No: 51A, Merkez/Tokat</a>
            </li>
            <li>
              <i class="fa-solid fa-phone icon"></i>
              <span>(0533) 249 06 99</span>
            </li>
            
          </ul>
        </div>

        <!-- Location 2 -->
        <div class="location-col">
          <h4 class="footer-title">Acil Durum</h4>
          <ul class="info-list">
            <li>
              <i class="fa-solid fa-truck-medical icon"></i>
              <span>7/24 Acil Servis Hizmetimiz Mevcuttur</span>
            </li>
            <li>
              <i class="fa-solid fa-phone icon"></i>
              <span>(0533) 249 06 99</span>
            </li>
          </ul>
        </div>
      </div>

      <div class="footer-bottom">
        <p>&copy; 2025 Atlas Veteriner Kliniği. Tüm hakları saklıdır.</p>
        <!-- <p class="developer-credit">
          Bu Web Sitesi <a href="https://www.linkedin.com/in/sercanturhan" target="_blank" class="dev-link">Sercan TURHAN</a> tarafından geliştirilmiştir.
        </p> -->
      </div>
    </div>
  </footer>
</template>

<style scoped>
.app-footer {
  background-color: white;
  padding-top: 5rem;
  padding-bottom: 2.5rem;
  border-top: 1px solid var(--paw-border);
}

.footer-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2.5rem;
  margin-bottom: 4rem;
}

/* Brand */
.brand-col {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.brand-logo {
  display: flex;
  align-items: center;
}

.logo-img {
  height: 60px;
  width: auto;
  object-fit: contain;
}

.brand-desc {
  color: var(--paw-gray);
  font-size: 0.875rem;
  line-height: 1.6;
}

.social-links {
  display: flex;
  gap: 1rem;
}

.social-link {
  width: 2.5rem;
  height: 2.5rem;
  background-color: var(--paw-bg);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--paw-dark);
  transition: all 0.3s;
}

.social-link:hover {
  background-color: var(--paw-orange);
  color: white;
}

/* Links & Locations */
.footer-title {
  font-weight: 700;
  font-size: 1.125rem;
  margin-bottom: 1.5rem;
  color: var(--paw-dark);
}

.footer-links {
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
  color: var(--paw-gray);
}

.footer-links a {
  transition: color 0.3s;
}

.footer-links a:hover {
  color: var(--paw-orange);
}

.info-list {
  display: flex;
  flex-direction: column;
  gap: 0.75rem;
  color: var(--paw-gray);
  font-size: 0.875rem;
}

.info-list li {
  display: flex;
  gap: 0.75rem;
}

.icon {
  color: var(--paw-orange);
  margin-top: 0.25rem;
}

/* Bottom */
.footer-bottom {
  border-top: 1px solid rgba(255,255,255,0.1);
  padding-top: 30px;
  text-align: center;
  color: var(--paw-gray);
  font-size: 0.9rem;
  display: flex;
  flex-direction: column;
  gap: 10px;
  align-items: center;
}

.dev-link {
  color: var(--paw-orange);
  font-weight: 600;
  transition: color 0.3s;
}

.dev-link:hover {
  color: white;
}

.bold {
  font-weight: 700;
  color: var(--paw-dark);
}

@media (max-width: 768px) {
  .footer-grid {
    grid-template-columns: 1fr;
    gap: 40px;
  }
}

@media (min-width: 768px) {
  .footer-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .footer-grid {
    grid-template-columns: repeat(4, 1fr);
  }
}
</style>
