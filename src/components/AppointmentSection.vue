<script setup>
// No script needed for simple display
</script>

<template>
  <section class="appointment-section" id="contact">
    <div class="container">
      <div class="appointment-box">
        <!-- Decorative Circles -->
        <div class="circle circle-1"></div>
        <div class="circle circle-2"></div>

        <div class="grid-layout">
          <!-- Info Side -->
          <div class="info-side">
            <h2 class="section-title">Hemen Randevu Alın</h2>
            <p class="section-desc">Minik dostunuz için hemen randevu oluşturun, uzman ekibimizle tanışın.</p>
            
            <ul class="benefits-list">
              <li class="benefit-item">
                <div class="icon-box">
                  <i class="fa-solid fa-user-doctor"></i>
                </div>
                <span>Uzman veteriner hekim kadrosu</span>
              </li>
              <li class="benefit-item">
                <div class="icon-box">
                  <i class="fa-solid fa-heart"></i>
                </div>
                <span>Sevgi dolu ve stressiz yaklaşım</span>
              </li>
              <li class="benefit-item">
                <div class="icon-box">
                  <i class="fa-solid fa-clock"></i>
                </div>
                <span>Hızlı ve acil müdahale imkanı</span>
              </li>
            </ul>
          </div>

          <!-- Phone Contact Side -->
          <div class="contact-wrapper">
            <div class="contact-card">
              <div class="phone-icon-large">
                <i class="fa-solid fa-phone-volume"></i>
              </div>
              <h3 class="contact-title">Bizi Arayın</h3>
              <p class="contact-text">Randevu ve bilgi almak için bize ulaşın</p>
              
              <a href="tel:05332490699" class="phone-link group">
                (0533) 249 06 99
                <i class="fa-solid fa-arrow-right arrow-icon"></i>
              </a>

              <!-- <div class="working-hours">
                <i class="fa-regular fa-clock"></i>
                <span>7/24 Acil Hizmet</span>
              </div> -->
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.appointment-section {
  padding: 6rem 0;
  background-color: var(--paw-bg);
}

.appointment-box {
  background-color: var(--paw-dark);
  color: white;
  border-radius: 2rem;
  padding: 3rem;
  position: relative;
  overflow: hidden;
  box-shadow: 0 20px 40px rgba(0,0,0,0.1);
}

.circle {
  position: absolute;
  background-color: var(--paw-orange);
  border-radius: 50%;
  filter: blur(80px);
  z-index: 0;
}

.circle-1 {
  top: -10rem;
  right: -10rem;
  width: 25rem;
  height: 25rem;
  opacity: 0.15;
}

.circle-2 {
  bottom: -5rem;
  left: -5rem;
  width: 20rem;
  height: 20rem;
  opacity: 0.1;
}

.grid-layout {
  position: relative;
  z-index: 10;
  display: grid;
  grid-template-columns: 1fr;
  gap: 4rem;
  align-items: center;
}

/* Info Side */
.section-title {
  font-size: 3rem;
  font-weight: 800;
  margin-bottom: 1.5rem;
  line-height: 1.2;
}

.section-desc {
  color: #D1D5DB;
  font-size: 1.125rem;
  margin-bottom: 3rem;
  line-height: 1.8;
}

.benefits-list {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.benefit-item {
  display: flex;
  align-items: center;
  gap: 1rem;
  font-weight: 500;
  font-size: 1.1rem;
}

.icon-box {
  width: 40px;
  height: 40px;
  background: rgba(255,255,255,0.1);
  border-radius: 12px;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--paw-orange);
}

/* Contact Wrapper Side */
.contact-wrapper {
  display: flex;
  justify-content: center;
}

.contact-card {
  background-color: white;
  border-radius: 2rem;
  padding: 3rem 2rem;
  width: 100%;
  max-width: 450px;
  text-align: center;
  color: var(--paw-dark);
  box-shadow: 0 20px 50px rgba(0,0,0,0.2);
  display: flex;
  flex-direction: column;
  align-items: center;
  transition: transform 0.3s ease;
}

.contact-card:hover {
  transform: translateY(-5px);
}

.phone-icon-large {
  width: 5rem;
  height: 5rem;
  background-color: rgba(58, 193, 247, 0.1);
  color: var(--paw-orange);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  font-size: 2rem;
  margin-bottom: 1.5rem;
}

.contact-title {
  font-size: 2rem;
  font-weight: 800;
  margin-bottom: 0.5rem;
}

.contact-text {
  color: var(--paw-gray);
  margin-bottom: 2rem;
}

.phone-link {
  display: inline-flex;
  align-items: center;
  gap: 1rem;
  font-size: 1.75rem;
  font-weight: 800;
  color: var(--paw-dark);
  padding: 1rem 2rem;
  background-color: var(--paw-bg);
  border-radius: 1rem;
  transition: all 0.3s;
  border: 2px solid transparent;
}

.phone-link:hover {
  background-color: var(--paw-orange);
  color: white;
  border-color: var(--paw-orange);
  box-shadow: 0 10px 20px rgba(58, 193, 247, 0.3);
}

.arrow-icon {
  font-size: 1.25rem;
  transition: transform 0.3s;
}

.phone-link:hover .arrow-icon {
  transform: translateX(5px);
}

.working-hours {
  margin-top: 2rem;
  display: flex;
  align-items: center;
  gap: 0.5rem;
  color: #16A34A; /* Green for available */
  font-weight: 600;
  background-color: #DCFCE7;
  padding: 0.5rem 1rem;
  border-radius: 9999px;
  font-size: 0.9rem;
}

@media (min-width: 1024px) {
  .appointment-box {
    padding: 5rem;
  }
  .grid-layout {
    grid-template-columns: 1fr 1fr;
    gap: 6rem;
  }
}
</style>
