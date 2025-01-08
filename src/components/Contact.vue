<template>
  <section id="contact" class="contact-section">
    <div class="contact-container">
      <h2 class="about-title">Contact Us</h2>
      <p class="contact-subtitle">We're here to help. Reach out to us for any inquiries or to schedule an appointment.</p>
      
      <div class="contact-content">
        <div class="contact-info">
          <div class="info-card">
            <h3>Contact Information</h3>
            <div class="info-item">
              <i class="fas fa-map-marker-alt"></i>
              <p>123 Therapy Lane<br>Mental Health City, MH 12345</p>
            </div>
            <div class="info-item">
              <i class="fas fa-phone"></i>
              <p>(123) 456-7890</p>
            </div>
            <div class="info-item">
              <i class="fas fa-envelope"></i>
              <p>info@butterflytherapy.com</p>
            </div>
          </div>
          
          <div class="social-links">
            <h3>Follow Us</h3>
            <div class="social-icons">
              <a href="#" class="social-icon">
                <i class="fab fa-facebook-f"></i>
              </a>
              <a href="#" class="social-icon">
                <i class="fab fa-twitter"></i>
              </a>
              <a href="#" class="social-icon">
                <i class="fab fa-instagram"></i>
              </a>
              <a href="#" class="social-icon">
                <i class="fab fa-linkedin-in"></i>
              </a>
            </div>
          </div>
        </div>

        <form class="contact-form">
          <div class="form-group">
            <input type="text" placeholder="Your Name" required>
          </div>
          <div class="form-group">
            <input type="email" placeholder="Your Email" required>
          </div>
          <div class="form-group">
            <input type="text" placeholder="Subject" required>
          </div>
          <div class="form-group">
            <textarea placeholder="Your Message" rows="5" required></textarea>
          </div>
          <button type="submit" class="submit-button">Send Message</button>
        </form>
      </div>
    </div>
  </section>
</template>

<script setup>
// Component logic will go here
</script>

<style scoped>
.contact-section {
  padding: 4rem 2rem;
  background-color: var(--background-color);
}

.contact-container {
  max-width: 1200px;
  margin: 0 auto;
}

.contact-subtitle {
  text-align: center;
  margin-bottom: 2rem;
  color: var(--text-color);
}

.contact-content {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
}

.contact-info {
  background-color: white;
  padding: 2rem;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
}

.info-card h3,
.social-links h3 {
  margin-bottom: 1.5rem;
  color: var(--primary-color);
}

.info-item {
  display: flex;
  align-items: center;
  margin-bottom: 1rem;
}

.info-item i {
  font-size: 1.2rem;
  color: var(--primary-color);
  margin-right: 1rem;
}

.social-icons {
  display: flex;
  gap: 1rem;
}

.social-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 40px;
  height: 40px;
  border-radius: 50%;
  background-color: var(--primary-color);
  color: white;
  transition: all 0.3s ease;
}

.social-icon:hover {
  background-color: var(--secondary-color);
  transform: translateY(-2px);
}

.contact-form {
  display: flex;
  flex-direction: column;
  gap: 1rem;
}

.form-group input,
.form-group textarea {
  width: 100%;
  padding: 0.75rem;
  border: 1px solid #ddd;
  border-radius: 4px;
  font-family: inherit;
}

.submit-button {
  background-color: var(--primary-color);
  color: white;
  padding: 0.75rem 2rem;
  border: none;
  border-radius: 25px;
  font-weight: bold;
  cursor: pointer;
  transition: all 0.3s ease;
}

.submit-button:hover {
  background-color: var(--secondary-color);
  transform: translateY(-2px);
}

@media (max-width: 768px) {
  .contact-content {
    grid-template-columns: 1fr;
  }
}
</style>
