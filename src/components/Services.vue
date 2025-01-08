<template>
  <section id="services" class="services-section">
    <h2 class="about-title">Our Services</h2>
    <div class="services-grid">
      <div class="service-card">
        <div class="service-icon">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <path d="M12 4a4 4 0 014 4c0 1.95-1.4 3.58-3.25 3.93L8 18h2v2H6v-1l.1-.14 2.35-6.52C7.19 9.89 6 8.54 6 7a4 4 0 014-4m0-2a6 6 0 00-6 6c0 2.97 2.16 5.43 5 5.91V19H8v2h8v-2h-3v-5.09c2.84-.48 5-2.94 5-5.91a6 6 0 00-6-6m-2 6c0-1.11.89-2 2-2s2 .9 2 2-.89 2-2 2-2-.89-2-2z"/>
          </svg>
        </div>
        <h3>Individual Therapy</h3>
        <p>Personalized one-on-one sessions tailored to your unique mental health needs. We specialize in:</p>
        <ul>
          <li>Anxiety and depression management</li>
          <li>Trauma recovery</li>
          <li>Stress reduction techniques</li>
          <li>Personal growth strategies</li>
        </ul>
      </div>

      <div class="service-card">
        <div class="service-icon">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm-1 15l-5-5 1.41-1.41L11 13.17l7.59-7.59L20 7l-9 9z"/>
          </svg>
        </div>
        <h3>Couples Therapy</h3>
        <p>Helping couples improve communication, resolve conflicts, and strengthen their bond. Our approach includes:</p>
        <ul>
          <li>Communication skills training</li>
          <li>Conflict resolution strategies</li>
          <li>Empathy and understanding enhancement</li>
          <li>Rebuilding trust and intimacy</li>
        </ul>
      </div>

      <div class="service-card">
        <div class="service-icon">
          <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
            <path d="M10 16.5v-1.58c0-.53.21-1.03.59-1.41l3.41-3.41c.78-.78.78-2.05 0-2.83s-2.05-.78-2.83 0l-3.41 3.41c-.78.78-.78 2.05 0 2.83s2.05.78 2.83 0l3.41-3.41c.38-.38.59-.88.59-1.41V7.5c0-.83-.67-1.5-1.5-1.5S9 6.67 9 7.5v1.58c0 .53-.21 1.03-.59 1.41l-3.41 3.41c-.78.78-.78 2.05 0 2.83s2.05.78 2.83 0l3.41-3.41c.78-.78.78-2.05 0-2.83s-2.05-.78-2.83 0l-3.41 3.41c-.38.38-.59.88-.59 1.41V16.5c0 .83.67 1.5 1.5 1.5s1.5-.67 1.5-1.5zM19 18h-4v-2h4v2zm0-4h-4v-2h4v2zm0-4h-4v-2h4v2zm0-4h-4v-2h4v2z"/>
          </svg>
        </div>
        <h3>Group Therapy</h3>
        <p>Supportive group sessions providing a sense of community and shared experience. Benefits include:</p>
        <ul>
          <li>Reduced feelings of isolation</li>
          <li>Diverse perspectives and feedback</li>
          <li>Development of interpersonal skills</li>
          <li>Cost-effective therapeutic environment</li>
        </ul>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  name: 'Services'
}
</script>

<style scoped>
.services-section {
  padding: 5rem 0;
  background-color: #f9f9f9;
  display: flex;
  flex-direction: column;
  align-items: center;
}

.about-title {
  font-size: 2.5rem;
  margin-bottom: 3rem;
  color: #333;
  text-align: center;
}

.services-grid {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
  gap: 2rem;
  width: 80%;
  max-width: 1200px;
}

.service-card {
  background-color: #fff;
  border-radius: 8px;
  padding: 2rem;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  display: flex;
  flex-direction: column;
  align-items: center;
  text-align: center;
}

.service-icon {
  display: flex;
  align-items: center;
  justify-content: center;
  width: 60px;
  height: 60px;
  margin-bottom: 1rem;
}

.service-icon svg {
  width: 100%;
  height: 100%;
  fill: #5cb85c; /* Example icon color */
}

h3 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #333;
}

p {
  font-size: 1rem;
  color: #666;
  margin-bottom: 1rem;
}

ul {
  list-style: none;
  padding: 0;
}

ul li {
  font-size: 0.9rem;
  color: #666;
  margin-bottom: 0.5rem;
}

/* Responsive design */
@media (max-width: 768px) {
  .services-grid {
    width: 95%;
    grid-template-columns: 1fr;
  }
}
</style>
