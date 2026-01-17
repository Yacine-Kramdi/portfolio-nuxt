<template>
  <section id="experiences" class="experiences-section">
    <div class="container">
      <div class="section-header">
        <h2 class="section-title">Mon Parcours Professionnel</h2>
        <p class="section-subtitle">Découvrez mes expériences et réalisations</p>
      </div>

      <div class="experiences-timeline">
        <div class="experience-item" v-for="experience in experiences" :key="experience.id">


          <div class="experience-content">
            <div class="experience-header">
              <div class="experience-image">
                <img :src="experience.image" :alt="experience.company" />
              </div>
              <h3 class="experience-title">{{ experience.title }}</h3>
              <span class="experience-company">{{ experience.company }}</span>
              <span class="experience-duration">{{ experience.duration }}</span>
            </div>

            <p class="experience-description"
              v-for="(point, index) in experience.description.split('- ').filter(p => p.trim())" :key="index">{{ point
              }}</p>

            <div class="experience-tech">
              <span class="tech-tag" v-for="stack in experience.stacks" :key="stack">{{ stack }}</span>
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
    title: "Full-stack Developer",
    company: "Université M'Hamed Bougara de Boumerdes -Stage",
    duration: 'Jan 2023 - Juil 2023',
    description: `- Développement de back office de l'application mobilité Boumerdes pour gérer différentes données.
- Développement de la plateforme mobilité de suivre les dossiers en ligne de stage à l'étranger pour les enseignants et les Ats plus les doctorants 'systeme de workflow ' qui facilite procédure par les responsables.
- Système de signature électronique des documents et aussi un système qui génère des attestations et de façon automatique pour faciliter la demande de visa et aussi la récupération des frais de stage par la banque à la fin de procédure.
- Un système de chat et aussi la suggestion des amis pour échanger des avis et rendre l'application utilisable aussi.`,
    image: '/images/Boumerdes.jpeg',
    stacks: ['Php', 'Mysql', 'JavaScript', 'Sql', 'Html', 'Css', 'Uikit']
  },
  {
    id: 2,
    title: 'Full-stack Developer',
    company: 'Techitaway',
    duration: 'Jan 2024 - Juil 2024',
    description: `- Participation à la maintenance de projets existants tels que "Gouny" et "Recordati", des projets basés en France, ainsi que d'autres projets locaux.
     - Résolution de divers problèmes liés au code, incluant la correction de bugs, l'optimisation des performances, et l'amélioration de la qualité du code pour assurer une meilleure stabilité et évolutivité des projets.`,
    image: '/images/techitaway.png',
    stacks: ['Laravel ', 'Postgresql', 'GitLab', 'Méthode agile', 'Ajax', 'Sharpoint api', 'Azure', 'Docker', 'Linux', "Travail d'équipe"]
  },
  {
    id: 3,
    title: 'Full-stack Developer',
    company: 'ITihad.group',
    duration: 'Juil 2024 - Août 2025',
    description: `- Au sein d’Itihad Group, j’ai été en charge de la maintenance et de l’optimisation de plusieurs sites web ainsi que de robots de scraping.
    - J’ai contribué à l’amélioration des performances front-end pour garantir une meilleure expérience utilisateur. 
    - J’ai également développé des pages en AMP (Accelerated Mobile Pages) afin d’optimiser le temps de chargement sur mobile et renforcer le SEO.`,
    image: '/images/itihad_group_logo.jpeg',
    stacks: ['Laravel ', 'Grattage de données', 'GitLab', 'Solr', 'Méthode agile', 'Ajax', 'Python', 'Docker', 'Linux', "Travail d'équipe", 'Résolution de problèmes', 'Amp', 'SEO', 'API REST', 'Nuxtjs', 'Vuejs']
  },
  {
    id: 3,
    title: "Ingénieur d'etudes et développement",
    company: 'Sonatrach',
    duration: 'Sept 2025 - Présent',
    description: ``,
    image: '/images/Sonatrach.svg',
    stacks: ['Oracle DB', 'Python', 'Django', 'Flask', 'API REST', 'travail d\'équipe', "Méthode agile", 'Communication']
  },
    {
    id: 4,
    title: 'Founder & CEO',
    company: 'Dziria',
    duration: 'Sept 2025 - Présent',
    description: "Dziria une plateforme high-tech d’achat et de vente en Algérie Offrir un espace simple et intuitif pour acheter, vendre et échanger. des produits neufs et d'occasion entre particuliers et professionnels.", 
    image: '/images/Dziria.png',
    stacks: ['Laravel','Nuxtjs','Elasticsearch', 'Postgresql', 'Docker', 'AWS', 'GitHub', 'Travail d\'équipe', 'Gestion de projet', 'Communication']
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

.experiences-timeline {
  display: flex;
  flex-direction: column;
  gap: 2rem;
  position: relative;
}


.experience-item {
  display: flex;
  gap: 1.5rem;
  position: relative;

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

  }

  .experience-item::before {}

  .experience-header {
    flex-direction: column;
    align-items: flex-start;
    gap: 0.5rem;
  }
}
</style>