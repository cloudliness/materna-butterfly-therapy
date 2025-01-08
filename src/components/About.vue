<template>
  <section id="about" class="about-section">
    <div class="about-container">
      <h2 class="about-title">About Christina</h2>
      <div class="about-content">
        <div class="about-image">
          <img src="/images/christina.jpeg" alt="Christina - Founder">
        </div>
        
        <div class="about-text">
          <div class="bio-section">
            <p>Helping and supporting others has always been my calling. Everyone has a unique story, and
whether sharing it comes easily or feels challenging, we all deserve a safe, non-judgmental
space to express ourselves.</p>

            <p>I'm Christina Cerroni, a Licensed Clinical Social Worker (LCSW) dedicated to guiding individuals through their mental health journeys. As a mother and a survivor of postpartum challenges and thyroid cancer, I understand the diverse paths of motherhood and the emotional complexities that accompany it. My own journey inspired my specialization in perinatal mental health.</p>
            
            <p>With years of experience working in community mental health clinics, social service agencies, and school-based mental health services, I have supported individuals facing anxiety, depression, trauma, and the unique challenges faced by foster families and youth. I believe it’s never too late to heal and overcome the obstacles we face. That’s why I’m here—to offer understanding and empathy that comes from both professional expertise and personal resilience.</p>
          </div>

          <div class="qualifications">
            <h4>Professional Background</h4>
            <ul>
              <li>Master's Degree in Clinical Psychology</li>
              <li>Certified Cognitive Behavioral Therapist</li>
              <li>Specialization in Anxiety and Depression</li>
              <li>Trauma-Informed Care Practitioner</li>
            </ul>
          </div>

          <div class="philosophy">
            <h4>Christina's Approach</h4>
              <p>"I believe in the power of transformation through compassionate, personalized care. My approach combines evidence-based techniques with a deep understanding of each individual's unique journey."</p>
              
              <p>Christina's therapeutic style is collaborative and tailored to each client's needs. She integrates various therapeutic modalities, including:</p>
              
              <ul>
                <li>Cognitive Behavioral Therapy (CBT)</li>
                <li>Mindfulness-Based Stress Reduction</li>
                <li>Solution-Focused Therapy</li>
                <li>Positive Psychology</li>
              </ul>
          </div>

        </div>
      </div>
    </div>
  </section>
</template>

<script setup>
// Component logic can be added here if needed
</script>

<style scoped>
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
  margin-bottom: 2rem;
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
  align-items: flex-start;
}

.about-image {
  flex: 1;
}

.about-image img {
  width: 100%;
  max-width: 400px;
  border-radius: 12px;
  box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.1), 0 2px 4px -1px rgba(0, 0, 0, 0.06);
}

.about-text {
  flex: 2;
  font-size: 1.1rem;
  line-height: 1.8;
  color: #4a5568;
}

.about-text h3 {
  font-size: 2rem;
  color: #2c3e50;
  margin-bottom: 1.5rem;
}

.about-text h4 {
  font-size: 1.5rem;
  color: #2c3e50;
  margin: 2rem 0 1rem;
}

.bio-section p {
  margin-bottom: 1.5rem;
}

.qualifications ul {
  list-style: none;
  padding: 0;
}

.qualifications li {
  margin-bottom: 0.8rem;
  padding-left: 1.5rem;
  position: relative;
}

.qualifications li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: #42b983;
  font-weight: bold;
}

.philosophy {
  margin: 2rem 0;
}

.philosophy h4 {
  margin: 2rem 0 1rem;
}

.philosophy p {
  margin-bottom: 1.5rem;
}

.philosophy ul {
  list-style: none;
  padding: 0;
}

.philosophy li {
  margin-bottom: 0.8rem;
  padding-left: 1.5rem;
  position: relative;
}

.philosophy li::before {
  content: '✓';
  position: absolute;
  left: 0;
  color: #42b983;
  font-weight: bold;
}

.stats {
  display: grid;
  grid-template-columns: repeat(auto-fit, minmax(150px, 1fr));
  gap: 1.5rem;
  margin-top: 2rem;
}

.stat-item {
  background: white;
  padding: 1.5rem;
  border-radius: 8px;
  box-shadow: 0 2px 4px rgba(0, 0, 0, 0.1);
  text-align: center;
}

.stat-number {
  display: block;
  font-size: 2rem;
  font-weight: bold;
  color: #42b983;
}

.stat-label {
  display: block;
  font-size: 0.9rem;
  color: #4a5568;
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
  
  .about-image img {
    max-width: 100%;
  }
  
  .stats {
    grid-template-columns: 1fr;
  }
}
</style>
