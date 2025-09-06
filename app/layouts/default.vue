<template>
  <div>
    <nav class="navbar">
      <div class="nav-container">
        <div class="nav-logo">
          <span class="logo-text">YK</span>
          <span class="logo-subtitle">Yacine Kramdi</span>
        </div>
        
        <ul class="nav-menu" :class="{ active: isMenuOpen }">
          <li class="nav-item">
            <a href="#home" class="nav-link" @click="closeMenu"> 
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3 9L12 2L21 9V20C21 20.5304 20.7893 21.0391 20.4142 21.4142C20.0391 21.7893 19.5304 22 19 22H5C4.46957 22 3.96086 21.7893 3.58579 21.4142C3.21071 21.0391 3 20.5304 3 20V9Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M9 22V12H15V22" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Accueil</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="#stacks" class="nav-link" @click="closeMenu"> 
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M17 7.82959C17.5826 7.93985 18.135 8.12762 18.647 8.38069M19 10.5903C19 10.8741 18.9737 11.1526 18.9229 11.4239M12.5 4.56023C12.5 4.25062 12.4135 3.9472 12.2497 3.68323C12.086 3.41925 11.8517 3.2044 11.5728 3.06205C11.2939 2.9197 10.9807 2.85522 10.6658 2.87567C10.3509 2.89612 10.0461 3.00078 9.78773 3.17853L3.78773 7.67853C3.29093 8.01221 3 8.56217 3 9.15038V17.8496C3 18.4378 3.29093 18.9878 3.78773 19.3215L9.78773 23.8215C10.0461 23.9992 10.3509 24.1039 10.6658 24.1243C10.9807 24.1448 11.2939 24.0803 11.5728 23.9379C11.8517 23.7956 12.086 23.5808 12.2497 23.3168C12.4135 23.0528 12.5 22.7494 12.5 22.4398V4.56023Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M18.5 15.5C19.9045 15.5 21.05 14.3545 21.05 12.95C21.05 11.5455 19.9045 10.4 18.5 10.4C17.0955 10.4 15.95 11.5455 15.95 12.95C15.95 14.3545 17.0955 15.5 18.5 15.5Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Stacks</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="#projets" class="nav-link" @click="closeMenu"> 
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M3 9C3 7.89543 3.89543 7 5 7H19C20.1046 7 21 7.89543 21 9V18C21 19.1046 20.1046 20 19 20H5C3.89543 20 3 19.1046 3 18V9Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M8 7V5C8 3.89543 8.89543 3 10 3H14C15.1046 3 16 3.89543 16 5V7" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M8 12H16" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M8 16H12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Projets</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="#experiences" class="nav-link" @click="closeMenu"> 
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M21 12C21 13.1819 20.7672 14.3522 20.3149 15.4442C19.8626 16.5361 19.1997 17.5282 18.364 18.364C17.5282 19.1997 16.5361 19.8626 15.4442 20.3149C14.3522 20.7672 13.1819 21 12 21C10.8181 21 9.64778 20.7672 8.55585 20.3149C7.46392 19.8626 6.47177 19.1997 5.63604 18.364C4.80031 17.5282 4.13738 16.5361 3.68508 15.4442C3.23279 14.3522 3 13.1819 3 12C3 9.61305 3.94821 7.32387 5.63604 5.63604C7.32387 3.94821 9.61305 3 12 3C14.3869 3 16.6761 3.94821 18.364 5.63604C20.0518 7.32387 21 9.61305 21 12Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M12 7V12L15 15" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Experiences</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="#formations" class="nav-link" @click="closeMenu"> 
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 6H20V18C20 19.1046 19.1046 20 18 20H6C4.89543 20 4 19.1046 4 18V6Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M4 6C4 4.89543 4.89543 4 6 4H18C19.1046 4 20 4.89543 20 6V6C20 7.10457 19.1046 8 18 8H6C4.89543 8 4 7.10457 4 6V6Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M8 12H16" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M8 8H16" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M8 16H12" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Formations</span>
            </a>
          </li>
          <li class="nav-item">
            <a href="#contact" class="nav-link" @click="closeMenu"> 
              <svg class="nav-icon" width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 4H20C21.1 4 22 4.9 22 6V18C22 19.1 21.1 20 20 20H4C2.9 20 2 19.1 2 18V6C2 4.9 2.9 4 4 4Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M22 6L12 13L2 6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
              <span>Contact</span>
            </a>
          </li>
        </ul>
        
        <div class="nav-social">
          <a href="https://www.linkedin.com/in/yacine-kramdi-642353217/" class="social-link">
            <i class="fab fa-linkedin-in"></i>
          </a>
          <a href="https://github.com/Yacine-Kramdi/" class="social-link">
            <i class="fab fa-github"></i>
          </a>
        </div>
        
        <button class="mobile-menu-btn" @click="toggleMenu" :class="{ active: isMenuOpen }">
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
  background: rgba(15, 23, 42, 0.95);
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
  height: 60px;
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
  gap: 1.5rem;
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
  z-index: 1001;
}

.mobile-menu-btn span {
  width: 24px;
  height: 2px;
  background: #cbd5e1;
  margin: 3px 0;
  transition: 0.3s;
  transform-origin: center;
}

.mobile-menu-btn.active span:nth-child(1) {
  transform: rotate(45deg) translate(5px, 5px);
}

.mobile-menu-btn.active span:nth-child(2) {
  opacity: 0;
}

.mobile-menu-btn.active span:nth-child(3) {
  transform: rotate(-45deg) translate(7px, -6px);
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
    background: rgba(15, 23, 42, 0.98);
    backdrop-filter: blur(10px);
    width: 100%;
    height: calc(100vh - 60px);
    padding: 1rem 0;
    border-top: 1px solid rgba(255, 255, 255, 0.1);
    transition: 0.3s;
    gap: 0;
    overflow-y: auto;
  }
  
  .nav-menu.active {
    left: 0;
  }
  
  .nav-item {
    width: 100%;
  }
  
  .nav-link {
    padding: 1.2rem 1.5rem;
    border-bottom: 1px solid rgba(255, 255, 255, 0.05);
    justify-content: flex-start;
  }
  
  .nav-social {
    display: none;
  }
  
  .logo-subtitle {
    display: none;
  }
}

/* Animation pour le menu mobile */
@keyframes slideIn {
  from {
    opacity: 0;
    transform: translateX(-20px);
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

.nav-menu.active .nav-item {
  animation: slideIn 0.3s ease forwards;
}

.nav-menu.active .nav-item:nth-child(1) { animation-delay: 0.1s; }
.nav-menu.active .nav-item:nth-child(2) { animation-delay: 0.15s; }
.nav-menu.active .nav-item:nth-child(3) { animation-delay: 0.2s; }
.nav-menu.active .nav-item:nth-child(4) { animation-delay: 0.25s; }
.nav-menu.active .nav-item:nth-child(5) { animation-delay: 0.3s; }
.nav-menu.active .nav-item:nth-child(6) { animation-delay: 0.35s; }
</style>

<script>
export default {
  data() {
    return {
      isMenuOpen: false
    }
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
      // Empêcher le défilement lorsque le menu est ouvert
      document.body.style.overflow = this.isMenuOpen ? 'hidden' : '';
    },
    closeMenu() {
      this.isMenuOpen = false;
      document.body.style.overflow = '';
    }
  }
}
</script>