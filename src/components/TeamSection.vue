<template>
  <section class="team-section" id="team">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Uzman Kadromuzla Tanışın</h2>
        <p class="section-desc">Sevimli dostlarınızın sağlığı ve mutluluğu için çalışan profesyonel ekibimiz.</p>
      </div>

      <div class="team-grid">
        <!-- Member 1 -->
        <div class="team-card group">
          <div class="image-wrapper">
            <img src="https://images.unsplash.com/photo-1559839734-2b71ea86b48e?q=80&w=800&auto=format&fit=crop" alt="Vet. Hekim Ayşe Yılmaz" class="member-img">
            <div class="social-overlay">
              <a href="#" class="social-btn"><i class="fa-brands fa-linkedin-in"></i></a>
              <a href="#" class="social-btn"><i class="fa-brands fa-twitter"></i></a>
            </div>
          </div>
          <h3 class="member-name">Vet. Hekim Ayşe Yılmaz</h3>
          <p class="member-role">Başhekim</p>
          <p class="member-bio">Dahiliye ve cerrahi alanında 10 yılı aşkın tecrübesiyle kliniğimizin kurucusu.</p>
        </div>

        <!-- Member 2 -->
        <div class="team-card group">
          <div class="image-wrapper">
            <img src="https://images.unsplash.com/photo-1612349317150-e413f6a5b16d?q=80&w=800&auto=format&fit=crop" alt="Vet. Hekim Mehmet Demir" class="member-img">
            <div class="social-overlay">
              <a href="#" class="social-btn"><i class="fa-brands fa-linkedin-in"></i></a>
              <a href="#" class="social-btn"><i class="fa-brands fa-facebook-f"></i></a>
            </div>
          </div>
          <h3 class="member-name">Vet. Hekim Mehmet Demir</h3>
          <p class="member-role">Cerrahi Uzmanı</p>
          <p class="member-bio">Ortopedik cerrahi ve acil müdahale konularında uzmanlaşmış hekimimiz.</p>
        </div>

        <!-- Member 3 -->
        <div class="team-card group">
          <div class="image-wrapper">
            <img src="https://images.unsplash.com/photo-1594824476969-513a7e02cc3d?q=80&w=800&auto=format&fit=crop" alt="Zeynep Kaya" class="member-img">
            <div class="social-overlay">
              <a href="#" class="social-btn"><i class="fa-brands fa-instagram"></i></a>
              <a href="#" class="social-btn"><i class="fa-brands fa-tiktok"></i></a>
            </div>
          </div>
          <h3 class="member-name">Zeynep Kaya</h3>
          <p class="member-role">Pet Kuaförü</p>
          <p class="member-bio">Dostlarınızın bakımı ve güzelliği için sevgiyle çalışan profesyonel kuaförümüz.</p>
        </div>
      </div>
    </div>
  </section>
</template>

<style scoped>
.team-section {
  padding: 6rem 0;
  background-color: white;
}

.section-header {
  text-align: center;
  max-width: 768px;
  margin: 0 auto 4rem;
}

.section-title {
  font-size: 2.5rem;
  font-weight: 800;
  margin-bottom: 1.5rem;
  color: var(--paw-dark);
}

.section-desc {
  font-size: 1.125rem;
  color: var(--paw-gray);
}

.team-grid {
  display: grid;
  grid-template-columns: 1fr;
  gap: 2rem;
}

.team-card {
  text-align: center;
}

.image-wrapper {
  position: relative;
  margin-bottom: 1.5rem;
  border-radius: 1.5rem;
  overflow: hidden;
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.1);
  transition: all 0.3s ease;
}

.team-card:hover .image-wrapper {
  box-shadow: 0 20px 25px -5px rgba(0, 0, 0, 0.1);
}

.member-img {
  width: 100%;
  aspect-ratio: 3/4;
  object-fit: cover;
  transition: transform 0.5s;
}

.team-card:hover .member-img {
  transform: scale(1.05);
}

.social-overlay {
  position: absolute;
  bottom: 1rem;
  left: 50%;
  transform: translateX(-50%) translateY(1rem);
  display: flex;
  gap: 0.75rem;
  opacity: 0;
  transition: all 0.3s ease;
}

.team-card:hover .social-overlay {
  opacity: 1;
  transform: translateX(-50%) translateY(0);
}

.social-btn {
  width: 2.5rem;
  height: 2.5rem;
  background-color: white;
  color: var(--paw-orange);
  border-radius: 50%;
  display: flex;
  align-items: center;
  justify-content: center;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
  transition: all 0.3s;
}

.social-btn:hover {
  background-color: var(--paw-orange);
  color: white;
}

.member-name {
  font-size: 1.5rem;
  font-weight: 700;
  margin-bottom: 0.25rem;
  color: var(--paw-dark);
}

.member-role {
  color: var(--paw-orange);
  font-weight: 700;
  font-size: 0.875rem;
  text-transform: uppercase;
  letter-spacing: 0.05em;
  margin-bottom: 0.75rem;
}

.member-bio {
  color: var(--paw-gray);
  font-size: 0.875rem;
  padding: 0 1rem;
  line-height: 1.6;
}

@media (min-width: 768px) {
  .team-grid {
    grid-template-columns: repeat(2, 1fr);
  }
}

@media (min-width: 1024px) {
  .section-title {
    font-size: 3rem;
  }
  .team-grid {
    grid-template-columns: repeat(3, 1fr);
  }
}
</style>
