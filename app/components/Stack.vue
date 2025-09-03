<template>
  <div class="skills-container">
    <div class="background-shapes">
      <div class="shape shape-1"></div>
      <div class="shape shape-2"></div>
      <div class="shape shape-3"></div>
    </div>

    <h2 class="skills-title">Mes Compétences Techniques</h2>
    <p class="skills-subtitle">Un aperçu de mes principales expertises et maîtrises</p>
    
    <div class="skills-grid">
      <div class="skill-card" v-for="stack in stacks" :key="stack.id">
        <div class="skill-header">
          <div class="skill-image">
            <img :src="stack.image" :alt="stack.name" />
          </div>
          <span class="skill-name">{{ stack.name }}</span>
          <span class="skill-percentage">{{ stack.pourcentage }}%</span>
        </div>
        
        <div class="progress-container">
          <div class="progress-bar">
            <div 
              class="progress-fill" 
              :style="{ width: stack.pourcentage + '%' }"
            ></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script setup>
const stacks = [
  { id: 1, name: 'HTML/CSS', image: 'https://cdn-icons-png.flaticon.com/512/732/732212.png', pourcentage: 90 },
  { id: 2, name: 'JavaScript', image: 'https://cdn-icons-png.flaticon.com/512/5968/5968292.png', pourcentage: 85 },
  { id: 3, name: 'Vue.js/Nuxt.js', image: 'https://nuxt.com/assets/design-kit/logo/icon-green.png', pourcentage: 88 },
  { id: 4, name: 'Node.js', image: 'https://cdn-icons-png.flaticon.com/512/919/919825.png', pourcentage: 75 },
  { id: 5, name: 'Base de données', image: 'https://cdn-icons-png.flaticon.com/512/4299/4299956.png', pourcentage: 82 },
  { id: 6, name: 'Docker', image: 'https://cdn-icons-png.flaticon.com/512/732/732212.png', pourcentage: 60 },
  { id: 7, name: 'Laravel', image: 'https://cdn-icons-png.flaticon.com/512/5968/5968292.png', pourcentage: 85 },
  { id: 8, name: 'Flutter', image: 'https://nuxt.com/assets/design-kit/logo/icon-green.png', pourcentage: 88 },
  { id: 9, name: 'Git', image: 'https://cdn-icons-png.flaticon.com/512/919/919825.png', pourcentage: 75 },
  { id: 10, name: 'Linux', image: 'https://cdn-icons-png.flaticon.com/512/4299/4299956.png', pourcentage: 82 },
  { id: 9, name: 'Php', image: 'https://cdn-icons-png.flaticon.com/512/919/919825.png', pourcentage: 75 },
  { id: 10, name: 'Python', image: 'https://cdn-icons-png.flaticon.com/512/4299/4299956.png', pourcentage: 82 },
  { id: 10, name: 'OpenCv', image: 'https://cdn-icons-png.flaticon.com/512/4299/4299956.png', pourcentage: 82 },
];
</script>

<style scoped>
.skills-container {
  min-height: 100vh;
  padding: 20px;
  position: relative;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  overflow: hidden;
}

.skills-title {
  font-size: 2.5rem;
  font-weight: 700;
  text-align: center;
  margin-bottom: 1rem;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.skills-subtitle {
  text-align: center;
  color: #94a3b8;
  margin-bottom: 3rem;
  font-size: 1.1rem;
}

.skills-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 1.5rem;
}

.skill-card {
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 1.5rem;
  transition: all 0.3s ease;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1);
}

.skill-card:hover {
  transform: translateY(-5px);
  box-shadow: 0 10px 15px -3px rgba(99, 102, 241, 0.2);
  border-color: rgba(99, 102, 241, 0.3);
}

.skill-header {
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
}

.skill-image {
  width: 40px;
  height: 40px;
  border-radius: 10px;
  display: flex;
  align-items: center;
  justify-content: center;
  background: rgba(255, 255, 255, 0.1);
  margin-right: 1rem;
  overflow: hidden;
}

.skill-image img {
  width: 24px;
  height: 24px;
  object-fit: contain;
}

.skill-name {
  flex: 1;
  font-weight: 600;
  color: #e2e8f0;
}

.skill-percentage {
  font-weight: 700;
  color: #6366f1;
}

.progress-container {
  width: 100%;
}

.progress-bar {
  width: 100%;
  height: 8px;
  background: rgba(255, 255, 255, 0.1);
  border-radius: 4px;
  overflow: hidden;
}

.progress-fill {
  height: 100%;
  border-radius: 4px;
  background: linear-gradient(90deg, #6366f1, #8b5cf6);
  transition: width 1s ease-in-out;
  position: relative;
}

.progress-fill::after {
  content: '';
  position: absolute;
  top: 0;
  left: 0;
  bottom: 0;
  right: 0;
  background-image: linear-gradient(
    -45deg,
    rgba(255, 255, 255, 0.2) 25%,
    transparent 25%,
    transparent 50%,
    rgba(255, 255, 255, 0.2) 50%,
    rgba(255, 255, 255, 0.2) 75%,
    transparent 75%,
    transparent
  );
  z-index: 1;
  background-size: 20px 20px;
  animation: move 1s linear infinite;
  border-radius: 4px;
}

@keyframes move {
  0% {
    background-position: 0 0;
  }
  100% {
    background-position: 20px 0;
  }
}

/* Responsive */
@media (max-width: 768px) {
  .skills-grid {
    grid-template-columns: 1fr;
  }
  
  .skills-title {
    font-size: 2rem;
  }
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
  top: 150px;
  right: -160px;
}

.shape-2 {
  width: 300px;
  height: 300px;
  background: linear-gradient(45deg, #ec4899, #f43f5e);
  bottom: 100px;
  left: -10%;
}

.shape-3 {
  width: 150px;
  height: 150px;
  background: linear-gradient(45deg, #10b981, #06b6d4);
  top: 70%;
  left: 50px;
}
</style>