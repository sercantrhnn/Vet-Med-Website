<template>
  <section class="hero-section" id="home">
    <!-- Background Shape -->
    <div class="bg-shape"></div>

    <div class="container">
      <div class="hero-grid">
        <!-- Content -->
        <div class="hero-content animate-fade-in-up">
          
            <!-- <i class="fa-solid fa-star text-yellow"></i>
            <span>Müşterilerimizden 4.9 puan</span> -->
          

          <h1 class="hero-title">
            Tokat'ta Profesyonel <span class="text-orange">Veteriner Hizmetleri</span>
          </h1>

          <p class="hero-desc">
            Atlas Veteriner Kliniği olarak, sevimli dostlarınızın sağlığı ve mutluluğu için uzman kadromuzla yanınızdayız. Modern tıbbi imkanlar ve sevgi dolu yaklaşımımızla hizmetinizdeyiz.
          </p>

          <div class="hero-actions">
            <a href="#contact" class="btn btn-primary btn-lg">
              Randevu Al
            </a>

            <div class="contact-info">
              <div class="phone-icon">
                <i class="fa-solid fa-phone"></i>
              </div>
              <div class="phone-text">
                <div class="phone-label">Bizi Arayın</div>
                <div class="phone-number">(0533) 249 06 99</div>
              </div>
            </div>
          </div>
        </div>

        <!-- Image -->
        <div class="hero-image-wrapper">
          <div class="blob-bg"></div>
          <div class="image-card">
            <img src="https://images.unsplash.com/photo-1516734212186-a967f81ad0d7?q=80&w=1000&auto=format&fit=crop" alt="Mutlu Köpek" class="hero-img">
            
            <!-- Floating Badge -->
            <div class="floating-badge">
              <div class="badge-icon">
                <i class="fa-solid fa-user-doctor"></i>
              </div>
              <div>
                <div class="badge-title">Uzman Bakım</div>
                <div class="badge-subtitle">Sertifikalı Hekimler</div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.hero-section {
  padding-top: 8rem;
  padding-bottom: 5rem;
  position: relative;
  overflow: hidden;
}

.bg-shape {
  position: absolute;
  top: 5rem;
  right: 0;
  width: 50%;
  height: 100%;
  background-color: rgba(58, 193, 247, 0.05); /* Updated to match new blue theme opacity */
  border-top-left-radius: 2rem;
  border-bottom-left-radius: 2rem;
  z-index: -1;
}

.hero-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 3rem;
  align-items: center;
}

/* Content */
.review-badge {
  display: inline-flex;
  align-items: center;
  gap: 0.5rem;
  padding: 0.5rem 1rem;
  background-color: white;
  border: 1px solid var(--paw-border);
  border-radius: 9999px;
  box-shadow: 0 1px 2px 0 rgba(0, 0, 0, 0.05);
  font-size: 0.875rem;
  font-weight: 700;
  color: var(--paw-dark);
  margin-bottom: 2rem;
}

.text-yellow {
  color: #FACC15;
}

.hero-title {
  font-size: 3rem;
  line-height: 1.1;
  font-weight: 800;
  color: var(--paw-dark);
  margin-bottom: 1.5rem;
}

.hero-desc {
  font-size: 1.125rem;
  color: var(--paw-gray);
  line-height: 1.6;
  margin-bottom: 2rem;
  max-width: 500px;
}

.hero-actions {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
  align-items: center;
}

.btn-lg {
  padding: 1rem 2rem;
  font-size: 1.125rem;
  box-shadow: 0 10px 40px -10px rgba(0,0,0,0.05);
}

.contact-info {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.phone-icon {
  width: 3rem;
  height: 3rem;
  background-color: white;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  color: var(--paw-orange);
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.phone-label {
  font-size: 0.875rem;
  color: var(--paw-gray);
  font-weight: 500;
}

.phone-number {
  font-weight: 700;
  color: var(--paw-dark);
}

/* Image Side */
.hero-image-wrapper {
  position: relative;
  display: flex;
  justify-content: center;
}

.blob-bg {
  position: absolute;
  inset: 0;
  background-color: rgba(58, 193, 247, 0.1); /* Updated to match new blue theme opacity */
  border-radius: 40% 60% 70% 30% / 40% 50% 60% 50%;
  transform: rotate(6deg) scale(1.05);
  z-index: 0;
}

.image-card {
  position: relative;
  z-index: 10;
  border-radius: 1.5rem;
  overflow: hidden;
  box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
  border: 4px solid white;
  transform: rotate(2deg);
  transition: transform 0.5s;
  max-width: 400px;
}

.image-card:hover {
  transform: rotate(0);
}

.hero-img {
  width: 100%;
  height: auto;
  display: block;
  aspect-ratio: 4/5;
  object-fit: cover;
}

.floating-badge {
  position: absolute;
  bottom: 2rem;
  left: 2rem;
  background-color: white;
  padding: 1rem;
  border-radius: 1rem;
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
  display: flex;
  align-items: center;
  gap: 1rem;
  max-width: 200px;
}

.badge-icon {
  background-color: #DCFCE7;
  color: #16A34A;
  padding: 0.75rem;
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
}

.badge-title {
  font-weight: 700;
  color: var(--paw-dark);
}

.badge-subtitle {
  font-size: 0.75rem;
  color: var(--paw-gray);
}

@media (min-width: 1024px) {
  .hero-section {
    padding-top: 12rem;
    padding-bottom: 8rem;
  }
  
  .hero-grid {
    grid-template-columns: 1fr 1fr;
    gap: 5rem;
  }

  .hero-content {
    text-align: left;
  }

  .hero-title {
    font-size: 4.5rem;
  }

  .hero-actions {
    flex-direction: row;
    justify-content: flex-start;
  }
}
</style>
