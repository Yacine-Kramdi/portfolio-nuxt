<template>
  <div id="home" class="portfolio-container">
    <div class="background-shapes">
      <div class="shape shape-1"></div>
      <div class="shape shape-2"></div>
      <div class="shape shape-3"></div>
    </div>
    
    <div class="profile-card">
      <div class="image-container">
        <img src="/images/profile.jpeg" alt="Photo de Yacine Kramdi" class="profile-img">
        <div class="image-overlay"></div>
      </div>
      
      <h1 class="name">Yacine Kramdi</h1>
      <h2 class="title">CEO & Fondateur – Dziria | Ingénieur de Développements Full Stack</h2>
      <p class="description">Créateur de solutions digitales innovantes alliant design et performance</p>
      
      <div class="cta-container">
        <button class="cta-button"  @click="downloadCV">
          <span>Télécharger mon CV</span>
          <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
            <path d="M12 16L12 4M12 16L8 12M12 16L16 12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            <path d="M4 20H20" stroke="currentColor" stroke-width="2" stroke-linecap="round"/>
          </svg>
        </button>
      </div>
      
      <div class="social-links">
        <a href="https://www.linkedin.com/in/yacine-kramdi-642353217/" class="social-link">
          <i class="fab fa-linkedin-in"></i>
        </a>
        <a href="https://github.com/Yacine-Kramdi/" class="social-link">
          <i class="fab fa-github"></i>
        </a>
        <a href="#" class="social-link">
          <i class="fab fa-twitter"></i>
        </a>
      </div>
    </div>
  </div>
</template>

<style scoped>
.portfolio-container {
  min-height: 100vh;
  display: flex;
  justify-content: center;
  align-items: center;
  padding: 20px;
  position: relative;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  overflow: hidden;
}

.background-shapes {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
  z-index: 1;
}

.shape {
  position: absolute;
  border-radius: 50%;
  opacity: 0.1;
}

.shape-1 {
  width: 300px;
  height: 300px;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  top: -150px;
  right: -150px;
}

.shape-2 {
  width: 200px;
  height: 200px;
  background: linear-gradient(45deg, #ec4899, #f43f5e);
  bottom: -100px;
  left: 10%;
}

.shape-3 {
  width: 150px;
  height: 150px;
  background: linear-gradient(45deg, #10b981, #06b6d4);
  top: 40%;
  left: -75px;
}

.profile-card {
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 24px;
  padding: 40px;
  text-align: center;
  box-shadow: 0 25px 50px -12px rgba(0, 0, 0, 0.25);
  max-width: 450px;
  width: 100%;
  z-index: 2;
  position: relative;
  overflow: hidden;
}

.profile-card::before {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  right: 0;
  height: 1px;
  background: linear-gradient(90deg, 
    rgba(255,255,255,0) 0%, 
    rgba(255,255,255,0.3) 50%, 
    rgba(255,255,255,0) 100%);
}

.image-container {
  position: relative;
  width: 150px;
  height: 150px;
  margin: 0 auto 20px;
}

.profile-img {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  object-fit: cover;
  position: relative;
  z-index: 2;
  box-shadow: 0 10px 25px -5px rgba(0, 0, 0, 0.3);
}

.image-overlay {
  position: absolute;
  top: -5px;
  left: -5px;
  right: -5px;
  bottom: -5px;
  background: linear-gradient(45deg, #6366f1, #8b5cf6, #ec4899);
  border-radius: 50%;
  z-index: 1;
  opacity: 0.7;
  filter: blur(10px);
}

.name {
  font-size: 28px;
  font-weight: 700;
  margin-bottom: 8px;
  background: linear-gradient(45deg, #fff, #cbd5e1);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.title {
  font-size: 18px;
  font-weight: 500;
  color: #94a3b8;
  margin-bottom: 16px;
}

.description {
  font-size: 16px;
  color: #cbd5e1;
  margin-bottom: 30px;
  line-height: 1.5;
}

.cta-container {
  margin-bottom: 30px;
}

.cta-button {
  display: inline-flex;
  align-items: center;
  justify-content: center;
  gap: 10px;
  padding: 14px 28px;
  font-size: 16px;
  font-weight: 600;
  color: #fff;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  border: none;
  border-radius: 12px;
  cursor: pointer;
  transition: all 0.3s ease;
  box-shadow: 0 4px 6px -1px rgba(99, 102, 241, 0.3), 0 2px 4px -1px rgba(99, 102, 241, 0.2);
}

.cta-button:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 15px -3px rgba(99, 102, 241, 0.4), 0 4px 6px -2px rgba(99, 102, 241, 0.25);
}

.cta-button:active {
  transform: translateY(0);
}

.social-links {
  display: flex;
  justify-content: center;
  gap: 16px;
}

.social-link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.05);
  color: #cbd5e1;
  transition: all 0.3s ease;
}

.social-link:hover {
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  color: #fff;
  transform: translateY(-2px);
}

/* Responsive */
@media (max-width: 480px) {
  .profile-card {
    padding: 30px 20px;
  }
  
  .name {
    font-size: 24px;
  }
  
  .title {
    font-size: 16px;
  }
}
</style>

<script>
export default {
  name: 'PortfolioHeader',
    methods: {
    downloadCV() {
      const link = document.createElement('a')
      link.href = '/Yacine_Kramdi_CV.pdf'
      link.setAttribute('download', 'Yacine-Kramdi-CV.pdf')
      document.body.appendChild(link)
      link.click()
      document.body.removeChild(link)
    }
  }
}
</script>