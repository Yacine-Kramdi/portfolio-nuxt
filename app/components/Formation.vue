<template>
  <section id="formations" class="formation-section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Mes Formation</h2>
        <p class="section-subtitle">Découvrez mes formations</p>
      </div>

      <div class="formations-timeline">
        <div class="formation-item" v-for="formation in formations" :key="formation.id">
          <div class="formation-content">
            <div class="formation-header">
              <h3 class="formation-title">{{ formation.title }}</h3>
              <span class="formation-school">{{ formation.school }}</span>
              <span class="formation-duration">{{ formation.duration }}</span>
            </div>

            <p class="formation-description">{{ formation.description }}</p>

            <div class="formation-tech">
            <span class="tech-tag" v-for="stack in formation.stacks" :key="stack">{{ stack }}</span>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
const formations = [


  {
    id: 2,
    title: 'Baccaluariat-Mathématique',
    school: 'Lycée Boukabous Ahemd',
    duration: 'Jan 2015 - Juin 2018',
    description: 'Module sur les Mathématiques et Physique',
    image: 'https://images.unsplash.com/photo-1577375729152-4c8b5fcda381?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80',
      stacks: ['Mathématique','Physique']
  },
  {
    id: 2,
    title: "Licence en ingénierie des système d'information et du logiciel",
    school: 'Université Mhamed Bougara de Boumerdes',
    duration: 'Oct 2018 - Sep 2021',
    description: "Licence ingénierie des systèmes d'information et du logiciel, programmation orientée objet et sécurité informatique.",
      stacks: ['Algorithm','C/C++','POO','Sql','UML']
  },
  {
    id: 1,
    title: "Master en Technologie de l'information",
    school: 'Université Mhamed Bougara de Boumerdes',
    duration: 'Oct 2021 - Juil 2023',
    description: "Module sur la programmation fonctionnelle, le réseau informatique plus la sécurité et l'intelligence artificielle.",
    image: 'https://images.unsplash.com/photo-1568992687947-868a62a9f521?ixlib=rb-4.0.3&ixid=M3wxMjA3fDB8MHxwaG90by1wYWdlfHx8fGVufDB8fHx8fA%3D%3D&auto=format&fit=crop&w=200&q=80',
    stacks: ['C/C++','POO','Sql','UML','Réseau','Sécurité']
  },
];
</script>

<style scoped>
.formation-section {
  padding: 5rem 1rem;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  color: #fff;
}

.container {
  max-width: 1200px;
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

.formations-timeline {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  position: relative;
}


.formation-image {
  flex-shrink: 0;
  width: 80px;
  height: 80px;
  border-radius: 12px;
  overflow: hidden;
  border: 2px solid rgba(255, 255, 255, 0.1);
}

.formation-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
}

.formation-content {
  flex: 1;
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 1.5rem;
  transition: all 0.3s ease;
}

.formation-content:hover {
  border-color: rgba(99, 102, 241, 0.3);
  box-shadow: 0 10px 15px -3px rgba(0, 0, 0, 0.2);
}

.formation-header {
  display: flex;
  flex-wrap: wrap;
  align-items: center;
  gap: 0.5rem 1rem;
  margin-bottom: 1rem;
}

.formation-title {
  font-size: 1.25rem;
  font-weight: 600;
  color: #e2e8f0;
  margin: 0;
}

.formation-school {
  color: #6366f1;
  font-weight: 500;
}

.formation-duration {
  background: rgba(99, 102, 241, 0.1);
  color: #6366f1;
  padding: 0.25rem 0.75rem;
  border-radius: 20px;
  font-size: 0.875rem;
  font-weight: 500;
}

.formation-description {
  color: #94a3b8;
  line-height: 1.6;
  margin-bottom: 1rem;
}

.formation-tech {
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
  .formations-timeline::before {
    left: 20px;
  }

  .formation-item {
    flex-direction: column;

  }

 
  .formation-header {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
}
</style>