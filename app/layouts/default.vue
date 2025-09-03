<template>
  <div>
    <nav class="navbar">
      <div class="nav-container">
        <div class="nav-logo">
          <span class="logo-text">YK</span>
          <span class="logo-subtitle">Portfolio</span>
        </div>
        
        <ul class="nav-menu">
          <li class="nav-item">
            <NuxtLink to="/" class="nav-link">
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M9 22V12H15V22" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Accueil</span>
            </NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink to="/about" class="nav-link">
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M20 21C20 19.1435 19.2625 17.363 17.9497 16.0503C16.637 14.7375 14.8565 14 13 14H11C9.14348 14 7.36301 14.7375 6.05025 16.0503C4.7375 17.363 4 19.1435 4 21" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M12 11C14.2091 11 16 9.20914 16 7C16 4.79086 14.2091 3 12 3C9.79086 3 8 4.79086 8 7C8 9.20914 9.79086 11 12 11Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>À propos</span>
            </NuxtLink>
          </li>
          <li class="nav-item">
            <NuxtLink to="/contact" class="nav-link">
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 4H20C21.1 4 22 4.9 22 6V18C22 19.1 21.1 20 20 20H4C2.9 20 2 19.1 2 18V6C2 4.9 2.9 4 4 4Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M22 6L12 13L2 6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Contact</span>
            </NuxtLink>
          </li>
        </ul>
        
        <div class="nav-social">
          <a href="#" class="social-link">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M16 8a6 6 0 0 1 6 6v7h-4v-7a2 2 0 0 0-2-2 2 2 0 0 0-2 2v7h-4v-7a6 6 0 0 1 6-6z"></path>
              <rect x="2" y="9" width="4" height="12"></rect>
              <circle cx="4" cy="4" r="2"></circle>
            </svg>
          </a>
          <a href="#" class="social-link">
            <svg width="18" height="18" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M12 0C5.374 0 0 5.373 0 12C0 17.302 3.438 21.8 8.207 23.387C8.806 23.498 9 23.126 9 22.81V20.576C5.662 21.302 4.967 19.16 4.967 19.16C4.421 17.773 3.634 17.404 3.634 17.404C2.545 16.659 3.717 16.675 3.717 16.675C4.922 16.759 5.556 17.912 5.556 17.912C6.626 19.746 8.363 19.216 9.048 18.909C9.155 18.134 9.466 17.604 9.81 17.305C7.145 17 4.343 15.971 4.343 11.374C4.343 10.063 4.812 8.993 5.579 8.153C5.455 7.85 5.044 6.629 5.696 4.977C5.696 4.977 6.704 4.655 8.997 6.207C9.954 5.941 10.98 5.808 12 5.803C13.02 5.808 14.047 5.941 15.006 6.207C17.297 4.655 18.303 4.977 18.303 4.977C18.956 6.629 18.545 7.85 18.421 8.153C19.191 8.993 19.656 10.063 19.656 11.374C19.656 15.983 16.849 16.998 14.177 17.295C14.607 17.667 15 18.397 15 19.517V22.81C15 23.129 15.192 23.504 15.801 23.386C20.566 21.797 24 17.3 24 12C24 5.373 18.627 0 12 0Z" fill="currentColor"/>
            </svg>
          </a>
        </div>
        
        <button class="mobile-menu-btn">
          <span></span>
          <span></span>
          <span></span>
        </button>
      </div>
    </nav>
    <NuxtPage />
  </div>
</template>

<style scoped>
.navbar {
  background: rgba(15, 23, 42, 0.8);
  backdrop-filter: blur(10px);
  border-bottom: 1px solid rgba(255, 255, 255, 0.1);
  position: sticky;
  top: 0;
  z-index: 1000;
  padding: 0.5rem 0;
}

.nav-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 1rem;
  display: flex;
  align-items: center;
  justify-content: space-between;
}

.nav-logo {
  display: flex;
  align-items: center;
  gap: 0.5rem;
}

.logo-text {
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  color: white;
  width: 40px;
  height: 40px;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  font-weight: 700;
  font-size: 1.2rem;
}

.logo-subtitle {
  color: #e2e8f0;
  font-weight: 600;
  font-size: 1.1rem;
}

.nav-menu {
  display: flex;
  list-style: none;
  gap: 2rem;
  margin: 0;
  padding: 0;
}

.nav-item {
  position: relative;
}

.nav-link {
  display: flex;
  align-items: center;
  gap: 0.5rem;
  color: #cbd5e1;
  text-decoration: none;
  font-weight: 500;
  padding: 0.75rem 0;
  transition: all 0.3s ease;
  position: relative;
}

.nav-link:hover {
  color: #ffffff;
}

.nav-link::after {
  content: '';
  position: absolute;
  bottom: 0;
  left: 0;
  width: 0;
  height: 2px;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  transition: width 0.3s ease;
}

.nav-link:hover::after {
  width: 100%;
}

.nav-link.router-link-active {
  color: #ffffff;
}

.nav-link.router-link-active::after {
  width: 100%;
}

.nav-icon {
  flex-shrink: 0;
}

.nav-social {
  display: flex;
  gap: 1rem;
}

.social-link {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 36px;
  height: 36px;
  border-radius: 50%;
  background: rgba(255, 255, 255, 0.05);
  color: #cbd5e1;
  transition: all 0.3s ease;
}

.social-link:hover {
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  color: #ffffff;
  transform: translateY(-2px);
}

.mobile-menu-btn {
  display: none;
  flex-direction: column;
  background: none;
  border: none;
  cursor: pointer;
  padding: 0.5rem;
}

.mobile-menu-btn span {
  width: 24px;
  height: 2px;
  background: #cbd5e1;
  margin: 2px 0;
  transition: 0.3s;
}

/* Responsive */
@media (max-width: 768px) {
  .mobile-menu-btn {
    display: flex;
  }
  
  .nav-menu {
    position: fixed;
    left: -100%;
    top: 60px;
    flex-direction: column;
    background: rgba(15, 23, 42, 0.95);
    backdrop-filter: blur(10px);
    width: 100%;
    padding: 1rem;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    transition: 0.3s;
    gap: 0;
  }
  
  .nav-menu.active {
    left: 0;
  }
  
  .nav-item {
    width: 100%;
  }
  
  .nav-link {
    padding: 1rem;
    border-bottom: 1px solid rgba(255, 255, 255, 0.05);
  }
  
  .nav-social {
    display: none;
  }
}
</style>

<script>
// Pour gérer le menu mobile
export default {
  mounted() {
    // Gestion du menu mobile (optionnel)
    const menuBtn = document.querySelector('.mobile-menu-btn');
    const menu = document.querySelector('.nav-menu');
    
    if (menuBtn && menu) {
      menuBtn.addEventListener('click', () => {
        menu.classList.toggle('active');
      });
    }
  }
}
</script>