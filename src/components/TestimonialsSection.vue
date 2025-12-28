<template>
  <section class="testimonials-section">
    <div class="container">
      <h2 class="section-title">Müşterilerimiz Ne Diyor?</h2>
      
      <div class="testimonials-grid">
        <!-- Review 1 -->
        <div class="review-card">
          <i class="fa-solid fa-quote-right quote-icon"></i>
          
          <div class="stars">
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
          </div>

          <h3 class="review-title">"Harika bir hizmet, köpeğimle çok ilgilendiler. Kesinlikle tavsiye ediyorum."</h3>

          <div class="user-info">
            <img src="https://randomuser.me/api/portraits/men/32.jpg" alt="User" class="user-img">
            <div>
              <div class="user-name">Ahmet Yılmaz</div>
              <div class="user-location">Tokat, Merkez</div>
            </div>
          </div>
        </div>

        <!-- Review 2 -->
        <div class="review-card">
          <i class="fa-solid fa-quote-right quote-icon"></i>
          
          <div class="stars">
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
            <i class="fa-solid fa-star"></i>
          </div>

          <h3 class="review-title">"Kedim Pamuk için en güvenilir adres. Atlas Veteriner Kliniği'ne teşekkürler!"</h3>

          <div class="user-info">
            <img src="https://randomuser.me/api/portraits/women/44.jpg" alt="User" class="user-img">
            <div>
              <div class="user-name">Ayşe Demir</div>
              <div class="user-location">Tokat, Karşıyaka</div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.testimonials-section {
  padding: 6rem 0;
  background-color: white;
}

.section-title {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 4rem;
  color: var(--paw-dark);
  text-align: center;
}

.testimonials-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}

.review-card {
  background-color: var(--paw-bg);
  padding: 2.5rem;
  border-radius: 1.5rem;
  position: relative;
}

.quote-icon {
  position: absolute;
  top: 2.5rem;
  right: 2.5rem;
  font-size: 2.5rem;
  color: var(--paw-orange);
  opacity: 0.2;
}

.stars {
  display: flex;
  gap: 0.25rem;
  color: #FACC15;
  font-size: 0.875rem;
  margin-bottom: 1.5rem;
}

.review-title {
  font-size: 1.5rem;
  font-weight: 700;
  line-height: 1.3;
  margin-bottom: 1.5rem;
  color: var(--paw-dark);
}

.user-info {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.user-img {
  width: 3rem;
  height: 3rem;
  border-radius: 50%;
}

.user-name {
  font-weight: 700;
  color: var(--paw-dark);
}

.user-location {
  font-size: 0.875rem;
  color: var(--paw-gray);
}

@media (min-width: 768px) {
  .testimonials-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .section-title {
    font-size: 3rem;
  }
}
</style>
