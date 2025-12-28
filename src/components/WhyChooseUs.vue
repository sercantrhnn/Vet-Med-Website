<template>
  <section class="why-choose-us" id="about">
    <div class="container">
      <div class="grid-layout">
        
        <!-- Image Grid -->
        <div class="image-grid-wrapper">
          <div class="image-grid">
            <img src="/1.jpeg" class="grid-img translate-y">
            <img src="/2.jpeg" class="grid-img">
            <img src="/3.jpeg" class="grid-img translate-y">
            <img src="/4.jpeg" class="grid-img">
          </div>
          
          <!-- Center Badge -->
          <!-- <div class="center-badge">
            <span class="badge-number">10+</span>
            <span class="badge-text">Yıllık Deneyim</span>
          </div> -->
        </div>

        <!-- Content -->
        <div class="content-side">
          <h2 class="section-title">Neden Atlas Veteriner Kliniği?</h2>
          <p class="section-desc">Tokat'ın en güvenilir veteriner kliniği olarak, can dostlarınıza kendi ailemizden biri gibi bakıyoruz.</p>

          <div class="features-list">
            <!-- Feature 1 -->
            <div class="feature-item">
              <div class="feature-icon">
                <i class="fa-solid fa-user-doctor"></i>
              </div>
              <div>
                <h4 class="feature-title">Uzman Veteriner Hekimler</h4>
                <p class="feature-text">Alanında uzman, deneyimli ve sürekli kendini geliştiren hekim kadrosu.</p>
              </div>
            </div>

            <!-- Feature 2 -->
            <div class="feature-item">
              <div class="feature-icon">
                <i class="fa-solid fa-heart"></i>
              </div>
              <div>
                <h4 class="feature-title">Sevgi Dolu Yaklaşım</h4>
                <p class="feature-text">Stresten uzak, sevgi ve şefkat dolu bir muayene ortamı.</p>
              </div>
            </div>

            <!-- Feature 3 -->
            <div class="feature-item">
              <div class="feature-icon">
                <i class="fa-solid fa-microscope"></i>
              </div>
              <div>
                <h4 class="feature-title">Modern Teknoloji</h4>
                <p class="feature-text">En son teknoloji teşhis ve tedavi cihazları ile donatılmış klinik.</p>
              </div>
            </div>
          </div>
        </div>

      </div>
    </div>
  </section>
</template>

<style scoped>
.why-choose-us {
  padding: 6rem 0;
  background-color: var(--paw-bg);
  overflow: hidden;
}

.grid-layout {
  display: grid;
  grid-template-columns: 1fr;
  gap: 4rem;
  align-items: center;
}

/* Image Grid */
.image-grid-wrapper {
  position: relative;
}

.image-grid {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}

.grid-img {
  width: 100%;
  height: 16rem;
  object-fit: cover;
  border-radius: 1rem;
}

.translate-y {
  transform: translateY(2rem);
}

.center-badge {
  position: absolute;
  top: 50%;
  left: 50%;
  transform: translate(-50%, -50%);
  background-color: var(--paw-orange);
  color: white;
  width: 8rem;
  height: 8rem;
  border-radius: 50%;
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  border: 4px solid white;
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
  z-index: 10;
}

.badge-number {
  font-size: 1.875rem;
  font-weight: 700;
}

.badge-text {
  font-size: 0.75rem;
  font-weight: 500;
  text-align: center;
}

/* Content Side */
.section-title {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 1.5rem;
  color: var(--paw-dark);
}

.section-desc {
  font-size: 1.125rem;
  color: var(--paw-gray);
  margin-bottom: 2.5rem;
}

.features-list {
  display: flex;
  flex-direction: column;
  gap: 2rem;
}

.feature-item {
  display: flex;
  gap: 1.5rem;
}

.feature-icon {
  width: 3.5rem;
  height: 3.5rem;
  background-color: white;
  border-radius: 50%;
  flex-shrink: 0;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--paw-orange);
  font-size: 1.25rem;
  border: 1px solid var(--paw-border);
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
}

.feature-title {
  font-size: 1.25rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
  color: var(--paw-dark);
}

.feature-text {
  color: var(--paw-gray);
}

@media (min-width: 1024px) {
  .grid-layout {
    grid-template-columns: 1fr 1fr;
    gap: 5rem;
  }
  .section-title {
    font-size: 3rem;
  }
}
</style>
