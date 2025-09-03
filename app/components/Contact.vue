<template>
  <section class="contact-section">
    <div class="container">
      <div class="section-header">
        <h1 class="section-title">Contactez-moi</h1>
        <p class="section-subtitle">Une question, un projet ? N'hésitez pas à me contacter</p>
      </div>
      
      <div class="contact-content">
        <form class="contact-form">
          <div class="form-row">
            <div class="form-group">
              <label for="prenom">Prénom</label>
              <input type="text" id="prenom" name="prenom" required />
              <div class="input-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M20 21C20 19.1435 19.2625 17.363 17.9497 16.0503C16.637 14.7375 14.8565 14 13 14H11C9.14348 14 7.36301 14.7375 6.05025 16.0503C4.7375 17.363 4 19.1435 4 21" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                  <path d="M12 11C14.2091 11 16 9.20914 16 7C16 4.79086 14.2091 3 12 3C9.79086 3 8 4.79086 8 7C8 9.20914 9.79086 11 12 11Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                </svg>
              </div>
            </div>
            
            <div class="form-group">
              <label for="name">Nom</label>
              <input type="text" id="name" name="name" required />
              <div class="input-icon">
                <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                  <path d="M19 21V5C19 3.89543 18.1046 3 17 3H7C5.89543 3 5 3.89543 5 5V21" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                  <rect x="5" y="3" width="14" height="18" rx="2" stroke="currentColor" stroke-width="2"/>
                </svg>
              </div>
            </div>
          </div>
          
          <div class="form-group">
            <label for="email">Email</label>
            <input type="email" id="email" name="email" required />
            <div class="input-icon">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 4H20C21.1 4 22 4.9 22 6V18C22 19.1 21.1 20 20 20H4C2.9 20 2 19.1 2 18V6C2 4.9 2.9 4 4 4Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M22 6L12 13L2 6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
          </div>
          
          <div class="form-group">
            <label for="message">Message</label>
            <textarea id="message" name="message" rows="5" required></textarea>
            <div class="input-icon">
              <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M21 15C21 15.5304 20.7893 16.0391 20.4142 16.4142C20.0391 16.7893 19.5304 17 19 17H7L3 21V5C3 4.46957 3.21071 3.96086 3.58579 3.58579C3.96086 3.21071 4.46957 3 5 3H19C19.5304 3 20.0391 3.21071 20.4142 3.58579C20.7893 3.96086 21 4.46957 21 5V15Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
          </div>
          
          <button type="submit" class="submit-btn">
            <span>Envoyer le message</span>
            <svg width="20" height="20" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M22 2L11 13" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              <path d="M22 2L15 22L11 13L2 9L22 2Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
            </svg>
          </button>
        </form>
        
        <div class="contact-info">
          <div class="info-card">
            <div class="info-icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M21 10C21 17 12 23 12 23C12 23 3 17 3 10C3 7.61305 3.94821 5.32387 5.63604 3.63604C7.32387 1.94821 9.61305 1 12 1C14.3869 1 16.6761 1.94821 18.364 3.63604C20.0518 5.32387 21 7.61305 21 10Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <circle cx="12" cy="10" r="3" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h3>Localisation</h3>
            <p>Alger, Algérie</p>
          </div>
          
          <div class="info-card">
            <div class="info-icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M4 4H20C21.1 4 22 4.9 22 6V18C22 19.1 21.1 20 20 20H4C2.9 20 2 19.1 2 18V6C2 4.9 2.9 4 4 4Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
                <path d="M22 6L12 13L2 6" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h3>Email</h3>
            <p>contact@yacinekramdi.com</p>
          </div>
          
          <div class="info-card">
            <div class="info-icon">
              <svg width="24" height="24" viewBox="0 0 24 24" fill="none" xmlns="http://www.w3.org/2000/svg">
                <path d="M22 16.92V19.92C22 20.52 21.49 21.03 20.92 21.05C20.26 21.08 19.33 21.11 18.2 21.11C10.47 21.11 4.11 14.75 4.11 7.02C4.11 5.89 4.14 4.96 4.17 4.3C4.19 3.73 4.7 3.22 5.3 3.22H8.3C8.67 3.22 8.99 3.46 9.09 3.82C9.22 4.27 9.38 4.83 9.5 5.21C9.59 5.5 9.5 5.81 9.26 6L7.79 7.47C9.06 10.08 11.19 12.2 13.79 13.48L15.26 12.01C15.45 11.82 15.72 11.72 16 11.72C16.04 11.72 16.09 11.72 16.13 11.73C16.5 11.84 17.06 12.01 17.52 12.14C17.88 12.24 18.12 12.56 18.12 12.93V15.93C18.12 16.32 17.86 16.66 17.48 16.77C17.07 16.89 16.51 17.05 16.06 17.18C15.75 17.27 15.48 17.49 15.41 17.81C15.3 18.33 15.18 19.01 15.12 19.46C15.05 19.99 15.52 20.44 16.05 20.44H19.05C20.15 20.44 21.05 19.54 21.05 18.44C21.05 17.31 21.04 16.92 22 16.92Z" stroke="currentColor" stroke-width="2" stroke-linecap="round" stroke-linejoin="round"/>
              </svg>
            </div>
            <h3>Téléphone</h3>
            <p>+213 XXX XX XX XX</p>
          </div>
        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Vous pouvez ajouter ici la logique de soumission du formulaire
</script>

<style scoped>
.contact-section {
  padding: 5rem 1rem;
  background: linear-gradient(135deg, #0f172a 0%, #1e293b 100%);
  color: #fff;
  min-height: 100vh;
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

.contact-content {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 3rem;
}

.contact-form {
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 2rem;
}

.form-row {
  display: grid;
  grid-template-columns: 1fr 1fr;
  gap: 1rem;
}

.form-group {
  position: relative;
  margin-bottom: 1.5rem;
}

.form-group label {
  display: block;
  margin-bottom: 0.5rem;
  font-weight: 500;
  color: #e2e8f0;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 0.75rem 1rem 0.75rem 2.5rem;
  background: rgba(255, 255, 255, 0.03);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 8px;
  color: #fff;
  font-size: 1rem;
  transition: all 0.3s ease;
}

.form-group input:focus,
.form-group textarea:focus {
  outline: none;
  border-color: #6366f1;
  box-shadow: 0 0 0 3px rgba(99, 102, 241, 0.2);
}

.input-icon {
  position: absolute;
  left: 0.75rem;
  top: 2.5rem;
  color: #94a3b8;
}

.form-group textarea {
  resize: vertical;
  min-height: 120px;
}

.submit-btn {
  display: flex;
  align-items: center;
  justify-content: center;
  gap: 0.5rem;
  width: 100%;
  padding: 1rem;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  color: white;
  border: none;
  border-radius: 8px;
  font-size: 1rem;
  font-weight: 600;
  cursor: pointer;
  transition: all 0.3s ease;
}

.submit-btn:hover {
  transform: translateY(-2px);
  box-shadow: 0 10px 15px -3px rgba(99, 102, 241, 0.4);
}

.contact-info {
  display: flex;
  flex-direction: column;
  gap: 1.5rem;
}

.info-card {
  background: rgba(255, 255, 255, 0.05);
  backdrop-filter: blur(10px);
  border: 1px solid rgba(255, 255, 255, 0.1);
  border-radius: 16px;
  padding: 1.5rem;
  transition: all 0.3s ease;
}

.info-card:hover {
  border-color: rgba(99, 102, 241, 0.3);
  transform: translateY(-5px);
}

.info-icon {
  width: 50px;
  height: 50px;
  border-radius: 12px;
  background: linear-gradient(45deg, #6366f1, #8b5cf6);
  display: flex;
  align-items: center;
  justify-content: center;
  margin-bottom: 1rem;
  color: white;
}

.info-card h3 {
  font-size: 1.25rem;
  font-weight: 600;
  margin-bottom: 0.5rem;
  color: #e2e8f0;
}

.info-card p {
  color: #94a3b8;
  margin: 0;
}

/* Responsive */
@media (max-width: 768px) {
  .contact-content {
    grid-template-columns: 1fr;
  }
  
  .form-row {
    grid-template-columns: 1fr;
  }
  
  .section-title {
    font-size: 2rem;
  }
}
</style>