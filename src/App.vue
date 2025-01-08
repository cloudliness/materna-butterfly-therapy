<template>
  <div class="app">
    <header class="header">
      <nav class="navbar">
        <div class="logo">Materna Butterfly Therapy</div>
        <ul class="nav-links">
          <li><a @click="scrollToSection('hero')" class="nav-link">Home</a></li>
          <li><a @click="scrollToSection('about')" class="nav-link">About</a></li>
          <li><a @click="scrollToSection('services')" class="nav-link">Services</a></li>
          <li><a @click="scrollToSection('contact')" class="nav-link">Contact</a></li>
        </ul>
      </nav>
    </header>

    <main>
      <section id="hero" class="hero-section">
        <div class="hero-content">
          <h1>Your Mental Health Matters</h1>
          <p>Find peace and balance in your life with our professional therapy services</p>
          <button class="cta-button">Get Started</button>
        </div>
      </section>

      <About />

      <Services />

      <Contact />
    </main>

    <footer class="footer">
      <div class="footer-content">
        <div class="footer-section">
          <h3>About Us</h3>
          <p>Providing compassionate mental health care since 2010. Our team is dedicated to helping you achieve personal growth and emotional well-being.</p>
        </div>

        <div class="footer-section">
          <h3>Quick Links</h3>
          <ul>
            <li><a @click="scrollToSection('hero')">Home</a></li>
            <li><a @click="scrollToSection('services')">Services</a></li>
            <li><a @click="scrollToSection('about')">About</a></li>
            <li><a @click="scrollToSection('contact')">Contact</a></li>
          </ul>
        </div>

        <div class="footer-section">
          <h3>Contact Info</h3>
          <p>123 Therapy Lane<br>Mental Health City, MH 12345</p>
          <p>Phone: (555) 123-4567</p>
          <p>Email: info@butterflytherapy.com</p>
        </div>

        <div class="footer-section">
          <h3>Follow Us</h3>
          <div class="social-links">
            <a href="#" class="social-link">Facebook</a>
            <a href="#" class="social-link">Twitter</a>
            <a href="#" class="social-link">Instagram</a>
            <a href="#" class="social-link">LinkedIn</a>
          </div>
        </div>
      </div>

      <div class="footer-bottom">
        <p>&copy; 2023 Butterfly Therapy. All rights reserved.</p>
        <p>Privacy Policy | Terms of Service</p>
      </div>
    </footer>
  </div>
</template>

<script setup>
import About from './components/About.vue';
import Contact from './components/Contact.vue'
import Services from './components/Services.vue';

const scrollToSection = (sectionId) => {
  const section = document.getElementById(sectionId)
  if (section) {
    section.scrollIntoView({
      behavior: 'smooth'
    })
  }
}
</script>

<style>
@import url('https://fonts.googleapis.com/css2?family=Quicksand:wght@400;500;600&display=swap');

/* Logo styling */
.logo {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 1.5rem;
  color: #2c3e50;
  letter-spacing: -0.5px;
  transition: all 0.3s ease;
}

.logo:hover {
  color: #42b983;
  transform: scale(1.02);
}

/* Navigation styling */
.nav-links {
  display: flex;
  gap: 2rem;
  list-style: none;
  margin: 0;
  padding: 0;
}

.nav-link {
  font-family: 'Quicksand', sans-serif;
  font-weight: 500;
  font-size: 1.1rem;
  color: #2c3e50;
  text-decoration: none;
  transition: all 0.3s ease;
  padding: 0.5rem 1rem;
  border-radius: 4px;
}

.nav-link:hover {
  color: #42b983;
  background-color: rgba(66, 185, 131, 0.1);
  transform: translateY(-2px);
}

/* Hero section styling */
.hero-section {
  min-height: 100vh;
  display: flex;
  align-items: center;
  justify-content: center;
  text-align: center;
  background: linear-gradient(rgba(0, 0, 0, 0.5), rgba(0, 0, 0, 0.5)), url('/images/christina.jpeg');
  background-size: cover;
  background-position: center;
  padding: 2rem;
}

.hero-content {
  max-width: 800px;
}

.hero-content h1 {
  font-family: 'Quicksand', sans-serif;
  font-weight: 600;
  font-size: 3.5rem;
  color: #ffffff;
  margin-bottom: 1.5rem;
  line-height: 1.2;
  text-shadow: 2px 2px 4px rgba(0, 0, 0, 0.3);
}

.hero-content p {
  font-family: 'Quicksand', sans-serif;
  font-weight: 400;
  font-size: 1.5rem;
  color: #ffffff;
  margin-bottom: 2.5rem;
  line-height: 1.6;
  text-shadow: 1px 1px 2px rgba(0, 0, 0, 0.3);
}

.cta-button {
  font-family: 'Quicksand', sans-serif;
  font-weight: 500;
  font-size: 1.2rem;
  padding: 1rem 2.5rem;
  border: none;
  border-radius: 4px;
  background-color: #42b983;
  color: #ffffff;
  cursor: pointer;
  transition: all 0.3s ease;
}

.cta-button:hover {
  background-color: #3aa876;
  transform: translateY(-2px);
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
}

/* Previous styles remain unchanged */

.footer {
  background-color: #2c3e50;
  color: #ffffff;
  padding: 4rem 2rem 2rem;
}

.footer-content {
  max-width: 1200px;
  margin: 0 auto;
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
  gap: 2rem;
  padding-bottom: 2rem;
}

.footer-section {
  margin-bottom: 2rem;
}

.footer-section h3 {
  color: #42b983;
  margin-bottom: 1.5rem;
  font-size: 1.2rem;
}

.footer-section p {
  line-height: 1.8;
  color: #f8f9fa;
}

.footer-section ul {
  list-style: none;
  padding: 0;
}

.footer-section ul li {
  margin-bottom: 1rem;
}

.footer-section ul li a {
  color: #f8f9fa;
  text-decoration: none;
  transition: color 0.2s ease;
}

.footer-section ul li a:hover {
  color: #42b983;
}

.social-links {
  display: flex;
  gap: 1rem;
  flex-wrap: wrap;
}

.social-link {
  color: #f8f9fa;
  text-decoration: none;
  transition: color 0.2s ease;
}

.social-link:hover {
  color: #42b983;
}

.footer-bottom {
  text-align: center;
  padding-top: 2rem;
  border-top: 1px solid rgba(255, 255, 255, 0.1);
  margin-top: 2rem;
}

.footer-bottom p {
  margin: 0.5rem 0;
  color: #f8f9fa;
  font-size: 0.9rem;
}

.footer-bottom a {
  color: #42b983;
  text-decoration: none;
}

@media (max-width: 768px) {
  .footer-content {
    grid-template-columns: 1fr;
  }
  
  .footer-section {
    text-align: center;
  }
  
  .social-links {
    justify-content: center;
  }

  .hero-content h1 {
    font-size: 2.5rem;
  }

  .hero-content p {
    font-size: 1.2rem;
  }
}

.about-section {
  padding: 6rem 2rem;
  background: linear-gradient(145deg, #f8f9fa, #ffffff);
}

.about-container {
  max-width: 1200px;
  margin: 0 auto;
  padding: 0 2rem;
}

.about-title {
  text-align: center;
  font-size: 2.5rem;
  margin-bottom: 3rem;
  position: relative;
  color: #2c3e50;
}

.about-title::after {
  content: '';
  width: 80px;
  height: 4px;
  background: #42b983;
  position: absolute;
  bottom: -15px;
  left: 50%;
  transform: translateX(-50%);
  border-radius: 2px;
}

.about-content {
  display: flex;
  gap: 4rem;
  align-items: center;
}

.about-text {
  flex: 2;
  font-size: 1.1rem;
  line-height: 1.8;
  color: #4a5568;
}

.about-text p {
  margin-bottom: 1.5rem;
}

.about-image {
  flex: 1;
  text-align: center;
  position: relative;
}

.about-image img {
  max-width: 100%;
  height: auto;
  border-radius: 12px;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
}

@media (max-width: 768px) {
  .about-content {
    flex-direction: column;
    gap: 2rem;
  }
  
  .about-title {
    font-size: 2rem;
  }
  
  .about-text {
    font-size: 1rem;
  }
}
</style>
