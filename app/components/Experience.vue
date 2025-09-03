<template>
  <section class="experiences-section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Mon Parcours Professionnel</h2>
        <p class="section-subtitle">Découvrez mes expériences et réalisations</p>
      </div>
      
      <div class="experiences-timeline">
        <div class="experience-item" v-for="experience in experiences" :key="experience.id">
          <div class="experience-image">
            <img :src="experience.image" :alt="experience.company" />
          </div>
          
          <div class="experience-content">
            <div class="experience-header">
              <h3 class="experience-title">{{ experience.title }}</h3>
              <span class="experience-company">{{ experience.company }}</span>
              <span class="experience-duration">{{ experience.duration }}</span>
            </div>
            
            <p class="experience-description">{{ experience.description }}</p>
            
            <div class="experience-tech">
              <span class="tech-tag">Vue.js</span>
              <span class="tech-tag">Nuxt</span>
              <span class="tech-tag">Node.js</span>
              <span class="tech-tag">MongoDB</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const experiences = [
  {
    id: 1,
    title: 'Développeur Full Stack',
    company: 'Company A',
    duration: 'Jan 2020 - Dec 2020',
    description: 'Développement d\'applications web modernes avec Vue.js et Node.js. Gestion de bases de données et mise en place d\'API RESTful.',
    image: 'https://images.unsplash.com/photo-1568992687947-868a62a9f521?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80'
  },
  {
    id: 2,
    title: 'Lead Développeur',
    company: 'Company B',
    duration: 'Jan 2021 - Présent',
    description: 'Encadrement d\'une équipe de développeurs pour créer des applications web évolutives. Architecture technique et revue de code.',
    image: 'https://images.unsplash.com/photo-1577375729152-4c8b5fcda381?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80'
  },
];
</script>

<style scoped>
.experiences-section {
  padding: 5rem 1rem;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  color: #fff;
}

.container {
  max-width: 1000px;
  margin: 0 auto;
}

.section-header {
  text-align: center;
  margin-bottom: 3rem;
}

.section-title {
  font-size: 2.5rem;
  font-weight: 700;
  margin-bottom: 0.5rem;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  background-clip: text;
}

.section-subtitle {
  color: #94a3b8;
  font-size: 1.1rem;
}

.experiences-timeline {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  position: relative;
}

.experiences-timeline::before {
  content: '';
  position: absolute;
  left: 40px;
  top: 0;
  bottom: 0;
  width: 2px;
  background: linear-gradient(to bottom, #6366f1, #8b5cf6);
}

.experience-item {
  display: flex;
  gap: 1.5rem;
  position: relative;
  padding-left: 40px;
}

.experience-item::before {
  content: '';
  position: absolute;
  left: 32px;
  top: 20px;
  width: 18px;
  height: 18px;
  border-radius: 50%;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  border: 3px solid #0f172a;
  z-index: 2;
}

.experience-image {
  flex-shrink: 0;
  width: 80px;
  height: 80px;
  border-radius: 12px;
  overflow: hidden;
  border: 2px solid rgba(255, 255, 255, 0.1);
}

.experience-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.experience-content {
  flex: 1;
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 1.5rem;
  transition: all 0.3s ease;
}

.experience-content:hover {
  border-color: rgba(99, 102, 241, 0.3);
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.2);
}

.experience-header {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0.5rem 1rem;
  margin-bottom: 1rem;
}

.experience-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: #e2e8f0;
  margin: 0;
}

.experience-company {
  color: #6366f1;
  font-weight: 500;
}

.experience-duration {
  background: rgba(99, 102, 241, 0.1);
  color: #6366f1;
  padding: 0.25rem 0.75rem;
  border-radius: 20px;
  font-size: 0.875rem;
  font-weight: 500;
}

.experience-description {
  color: #94a3b8;
  line-height: 1.6;
  margin-bottom: 1rem;
}

.experience-tech {
  display: flex;
  flex-wrap: wrap;
  gap: 0.5rem;
}

.tech-tag {
  padding: 0.25rem 0.75rem;
  background: rgba(99, 102, 241, 0.1);
  color: #6366f1;
  border-radius: 20px;
  font-size: 0.75rem;
  font-weight: 500;
}

/* Responsive */
@media (max-width: 768px) {
  .experiences-timeline::before {
    left: 20px;
  }
  
  .experience-item {
    flex-direction: column;
    padding-left: 30px;
  }
  
  .experience-item::before {
    left: 14px;
  }
  
  .experience-header {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
}
</style>