<template>
  <section id="profile">
    <div class="container4">
      <div class="profile-content">
        <div class="profile-image">
          <img src="@/assets/prof1.jpg" alt="Mateo Rumac" />
        </div>
        <div class="profile-info">
          <h2 id="tittle">Mateo Rumac</h2>
          <p class="subtext"><i>Univ. Bacc. Inf. </i></p> <br>
          <p class="description">Passionate web developer specializing in  modern frontend development</p> <br>
          <p class="description">Committed to delivering elegant and efficient  solutions that elevate user experiences</p> 
        </div>
      </div>
    </div>
  </section>

  <section id="projects">
    <div class="container2">
      <h2>Featured Projects</h2>
      <div class="cards-container">
        <div class="card">
          <div class="card-image">
            <a href="https://smartstyleecom.vercel.app/" target="_blank">
              <img src="@/assets/smartstyle.jpg" alt="E-commerce web app" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">SmartStyle</h3>
            <p class="cardtext">
              SmartStyle is a sleek e-commerce web application built with React, 
              designed to simplify online shopping. Leveraging a dynamic product API, SmartStyle offers a seamless and user-friendly experience, 
              with responsive design for optimal browsing on any device.
            </p>
          </div>
        </div>
        <div class="card">
          <div class="card-image">
            <a href="https://bbuddy-mateorumacs-projects.vercel.app/" target="_blank">
              <img src="@/assets/bbuddy.jpg" alt="Food search web app" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">BiteBuddy</h3>
            <p class="cardtext">
              BiteBuddy is an intuitive web application crafted with Vue.js, designed to make searching for food and recipes a breeze. Leveraging the powerful Spoonacular API, 
              BiteBuddy offers a seamless and feature-rich experience for food enthusiasts. <br><br>
              Note: API is limited to 150 requests per day.
            </p>
          </div>
        </div>
        <div class="card">
          <div class="card-image">
            <a href="https://frontend-wa.vercel.app" target="_blank">
              <img src="@/assets/bba.png" alt="Beauty salon website" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">Beauty by Ana</h3>
            <p class="cardtext">
              A beauty salon website featuring a fully functional backend to seamlessly handle user requests.<br /> <br> 
              Login to see more functionalities!<br>
              E-mail: user@gmail.com <br>
              Password: user1 <br><br>
              Note: Backend takes up to a minute to process requests due to inactivity.
            </p>
          </div>
        </div>
        <div class="card">
          <div class="card-image">
            <a href="https://pizzeria-jupiter.vercel.app/" target="_blank">
              <img src="@/assets/pizzeria.jpg" alt="Pizzeria Jupiter" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">Pizzeria Jupiter</h3>
            <p class="cardtext">
              A modernized pizza restaurant website for Pizzeria Jupiter, skillfully redesigned using Vue.js to enhance user experience and streamline functionality.
            </p>
          </div>
        </div>
        <div class="card">
          <div class="card-image">
            <a href="https://github.com/mateorumac/userManagement" target="_blank">
              <img src="@/assets/users.png" alt="User management dashboard" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">User management dashboard</h3>
            <p class="cardtext">
              A React app for managing users, featuring a searchable, paginated user table. Users can be edited or deleted with simple controls. The app offers responsive design and efficient user data management.
            </p>
          </div>
        </div>
        <!-- Add more cards -->
      </div>
    </div>
  </section>
  <section id="publications">
    <div class="container2">
      <h2>Published Work</h2>
      <div class="cards-container">
        <div class="card vertical-card">
          <div class="card-image">
            <a href="https://repozitorij.unipu.hr/islandora/object/unipu%3A9707" target="_blank">
              <img src="@/assets/zavrsnirad.png" alt="Paper Title Image" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">Artificial intelligence and web frontend programming</h3>
            <p class="cardtext short-text">
              This paper examines how AI, especially tools like ChatGPT and Copilot, can enhance frontend web development. 
              It highlights their impact on user experience and development speed.
              Future trends like Edge AI and generative models are discussed, along with challenges such as performance 
              optimization and user privacy. Practical examples show AI's growing role in creating smarter web applications.
            </p>
            <p class="keywords">Keywords: Artificial intelligence, Frontend programming, ChatGPT, Copilot, web applications</p>
          </div>
        </div>
      </div>
    </div>
  </section>
  <section id="about">
  <div class="container5">
    <h2>A Bit About Me</h2> <br>
    <div class="about-cards">
      <!-- Card 1 -->
      <div class="about-card">
        <i class="fas fa-user-graduate"></i>
        <h3>Education</h3>
        <p>
          I'm Mateo Rumac, a 24-year-old web developer employed at D&A Nekretnine. I graduated from Juraj Dobrila University in Pula, Croatia, where I honed my skills in modern web technologies and design.
        </p>
      </div>
      <!-- Card 2 -->
      <div class="about-card">
        <i class="fas fa-language"></i>
        <h3>Language Skills</h3>
        <p>
          I am fluent in English with a C1 proficiency, allowing me to communicate effectively and handle both technical and client-facing aspects of projects.
        </p>
      </div>
      <!-- Card 3 -->
      <div class="about-card">
        <i class="fas fa-briefcase"></i>
        <h3>Professional Services</h3>
        <p>
          In addition to my professional role, I am available to create websites for clients. I take pride in delivering elegant and efficient solutions tailored to individual needs.
        </p>
      </div>
    </div>
    <button class="dwnldbtn" @click="visitResumeSite">View Resume</button>
  </div>
</section>
  <section id="cta">
    <div class="container3">
      <h2>Ready to bring your vision to life?</h2>
      <p>
        I’d love to hear from you! Whether you have a project in mind or are looking to collaborate, feel free to reach out through any of my channels. Let’s create something amazing together.
      </p>
      <div class="contact-links">
        <div class="contact-item">
          <a href="mailto:mateo.rumac@gmail.com" class="contact-item" title="Email">
            <i class="fas fa-envelope"></i>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://www.linkedin.com/in/mateo-rumac-170a0b304/" target="_blank" class="contact-item">
            <i class="fab fa-linkedin"></i>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://www.instagram.com/rooksoni/" target="_blank" class="contact-item">
            <i class="fab fa-instagram"></i>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://github.com/mateorumac" target="_blank" class="contact-item">
            <i class="fab fa-github"></i>
          </a>
        </div>
      </div>
      <div class="footer">
        <p>© 2024 MATEO RUMAC | ALL RIGHTS RESERVED</p>
      </div>
    </div>
  </section>
</template>

<script>
import '@fortawesome/fontawesome-free/css/all.css';

export default {
  data() {
    return {
      showHero: false,
    };
  },
  mounted() {
    setTimeout(() => {
      this.showHero = true; 
    }, 500); 
  },
  methods: {
    visitDifferentSite() {
      const url = 'https://github.com/mateorumac/frontendWA';
      window.open(url, '_blank');
    },
    visitResumeSite() {
      const url = 'https://mateorumaccveng.tiiny.site/';
      window.open(url, '_blank');
    },
  },
  };
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');

@keyframes fadeInLeft {
  from {
    opacity: 0;
    transform: translateX(-50px); 
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadeInRight {
  from {
    opacity: 0;
    transform: translateX(50px); 
  }
  to {
    opacity: 1;
    transform: translateX(0);
  }
}

@keyframes fadeInUp {
  from {
    opacity: 0;
    transform: translateY(50px); 
  }
  to {
    opacity: 1;
    transform: translateY(0);
  }
}

/* Image animation */
.profile-image img {
  animation: fadeInLeft 1.5s ease-out; 
  opacity: 0; 
  animation-fill-mode: forwards; 
}

/* Text animation */
.profile-info {
  animation: fadeInRight 1.5s ease-out 0.5s; 
  opacity: 0; 
  animation-fill-mode: forwards; 
}

h1 {
  font-size: 3.5rem;
  margin: 0;
  font-family: 'Roboto Slab', serif;
  color: #c9b373; 
}

.subtext {
  font-size: 1.3rem; 
  color: #f8f5e1; 
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  margin-top: -1.3rem;
}

#tittle {
  font-size: 2.4rem;
  text-align: center;
}

.description {
  font-size: 1.25rem; 
  color: #f8f5e1; 
  line-height: 1.6; 
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  margin-top: 0.8rem;
}

#cta {
  background-color: #1E1E1E; 
  text-align: center;
  padding: 50px;
  position: relative;
}

.container3 {
  max-width: 800px;
  margin: 0 auto;
}

h2 {
  font-size: 2.2rem;
  margin-bottom: 1rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  color: #c9b373; 
}

p {
  font-size: 1.25rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  color: #f8f5e1; 
}

.cardtext {
  font-size: 1.25rem;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  color: #1E1E1E;
}

#profile {
  background: linear-gradient(135deg, #2c2c2c, #1E1E1E); 
  padding: 4rem 0;
  color: #f8f5e1;
}

.container4 {
  max-width: 1600px; 
  margin: 0 auto; 
  display: flex;
  justify-content: space-between; 
  align-items: center; 
  padding: 0; 
  gap: 4rem;
}

.profile-content {
  display: flex;
  justify-content: flex-start; 
  align-items: center;
  flex-wrap: nowrap; 
  gap: 4rem;
}

.profile-image img {
  flex-shrink: 0;
  width: 550px; 
  height: auto; 
  border-radius: 15px; 
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3); 
  margin-left: -180px;
}

.profile-image img:hover {
  transform: scale(1.05); 
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
}

.profile-info {
  flex: 1; 
  max-width: 1000px; 
  text-align: center; 
  line-height: 2; 
  font-size: 1.3rem; 
  color: #f8f5e1;
}

#projects {
  background-color: #1E1E1E;
  padding: 4rem 0;
  color: #f4f4f4;
  text-align: center;
}

.cards-container {
  margin-top: 4rem;
  display: flex;
  flex-direction: column;
  gap: 5rem;
  align-items: center;
}

.card {
  position: relative;
  display: flex;
  flex-direction: row; 
  align-items: center;
  background-color: #2c2c2c;
  border-radius: 15px;
  padding: 20px;
  width: 80%;
  max-width: 1200px;
  height: 400px; 
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
}

.card:hover {
  transform: scale(1.05);
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.5);
}

.card::before, .card::after {
  content: '';
  position: absolute;
  width: 80px;
  height: 80px;
  border: 2px solid #c9b373;
  z-index: 1;
  transition: transform 0.3s ease;
}

.card::before {
  top: -20px;
  left: -20px;
  transform: rotate(45deg);
}

.card::after {
  bottom: -20px;
  right: -20px;
  transform: rotate(45deg);
}

.card-image {
  width: 50%; 
  height: 100%;
  padding-right: 20px;
}

.card-image img {
  width: 100%;
  height: 100%;
  object-fit: cover;
  border-radius: 15px; 
  transition: transform 0.3s ease;
}

.card-content {
  width: 50%;
  padding: 0 20px;
  display: flex;
  flex-direction: column;
  justify-content: center;
}

.project-headline {
  font-family: 'Montserrat', sans-serif;
  font-weight: 700;
  font-size: 1.8rem;
  color: #c9b373; 
  margin-bottom: 1rem;
}

.cardtext {
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  font-size: 1.1rem;
  line-height: 1.6;
  color: #f4f4f4;
}

.container2 {
  margin-bottom: 2rem; 
}

#publications {
  background-color: #1E1E1E;
  padding: 4rem 0;
  color: #f4f4f4;
  text-align: center;
}


#about {
  background-color: #2c2c2c; 
  padding: 4rem 0;
}

.about-cards {
  display: flex;
  justify-content: center; 
  align-items: stretch; 
  gap: 2rem; 
  flex-wrap: nowrap; 
  margin-top: 2rem;
}

.about-card {
  background-color: #1E1E1E;
  color: #f8f5e1;
  border-radius: 10px;
  padding: 1.5rem;
  width: 300px; 
  height: 350px; 
  text-align: center;
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3);
  transition: transform 0.3s ease, box-shadow 0.3s ease;
  display: flex;
  flex-direction: column;
  justify-content: space-between; 
  flex-shrink: 0; 
}

.about-card:hover {
  transform: scale(1.05);
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.5);
}

.about-card i {
  font-size: 2.5rem;
  color: #c9b373;
  margin-bottom: 1rem;
}

.about-card h3 {
  font-size: 1.5rem;
  margin-bottom: 1rem;
  color: #c9b373;
}

.about-card p {
  font-size: 1rem;
  line-height: 1.6;
  color: #f8f5e1;
  flex-grow: 1; 
  display: flex;
  align-items: center; 
  justify-content: center; 
  margin: 0;
}

.dwnldbtn {
  display: block;
  margin-top: 3rem !important; 
  margin-left: auto;
  margin-right: auto;
  background-color: #c9b373;
  color: #1E1E1E;
  padding: 16px;
  text-decoration: none;
  font-size: 1.1rem;
  border-radius: 5px;
  transition: background-color 0.3s, transform 0.3s ease-in-out;
  border: none;
  outline: none;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  text-align: center;
}

.dwnldbtn:hover {
  background-color: #b2955d;
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}
.container5 {
  max-width: 800px;
  margin: 0 auto;
}

.aboutme {
  font-size: 1.25rem;
  text-align: center;
  margin-top: 10px;
  padding-top: 10px;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
  color: #f8f5e1; 
}

#about h2 {
  color: #c9b373; 
}

.dwnldbtn {
  display: inline-block;
  background-color: #c9b373;
  color: #1E1E1E;
  padding: 16px;
  margin-top: 10px;
  text-decoration: none;
  font-size: 1.1rem;
  border-radius: 5px;
  transition: background-color 0.3s, transform 0.3s ease-in-out;
  border: none; 
  outline: none;
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
}

.dwnldbtn:hover {
  background-color: #b2955d;
  transform: scale(1.05);
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.2);
}

.contact-links {
  display: flex;
  justify-content: center;
}

.contact-item {
  margin: 0 10px;
  text-decoration: none;
  font-size: 2rem;
  transition: color 0.3s ease;
  cursor: pointer;
  color: #c9b373;
}

.contact-item:hover {
  color: #f4f4f4;
}

.footer {
  margin-top: 20px;
  text-align: center; 
}

.footer p {
  margin: 0;
  font-size: 0.8rem;
  color: #F4F4F4; 
  font-family: 'Montserrat', sans-serif;
  font-weight: 400;
}

/* Larger screens */
@media only screen and (min-width: 1200px) {
  .container4,
  .container5,
  .container3 {
    max-width: 800px;
    margin: 0 auto;
  }

  .profile-content {
    flex-direction: row; 
    justify-content: space-between;
  }

  .profile-info {
    max-width: 60%;
    margin-left: 80px;
  }

  .project-content {
    margin-left: 0;
  }

  .project-image img {
    max-width: 110%; 
    border-radius: 8px;
    margin-left: 30px;
    padding: 10px;
  }

  .project-info {
    max-width: 60%; 
    padding: 20px;
    font-family: 'Roboto Slab', serif;
  }

  .container2 {
    max-width: none;
  }

  #about .about-cards {
    flex-wrap: nowrap; 
    justify-content: center;
    gap: 3rem; 
  }

  #about .about-card {
    width: 300px; 
    height: 350px; 
  }

  .dwnldbtn {
    margin-top: 3rem; 
  }
}

/* Medium screens */
@media only screen and (min-width: 1024px) and (max-width: 1440px) {
  .container4,
  .container5,
  .container3 {
    max-width: 900px;
    margin: 0 auto;
  }

  .profile-content {
    flex-direction: row;
    justify-content: space-between;
  }

  .profile-info {
    max-width: 50%; 
    margin-left: 50px;
  }

  .profile-image img {
    width: 100%; 
    margin-left: -30px; 
  }

  .cards-container {
    display: flex;
    flex-direction: column;
    gap: 5rem;
    align-items: center; 
    padding: 0 20px; 
  }

  .card {
    height: auto;
    width: 100%; 
    max-width: 900px; 
    margin: 0 auto; 
  }

  .card-image {
    width: 100%; 
    height: 250px; 
  }

  .card-content {
    width: 100%;
    padding: 0 10px;
  }

  header .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  .nav-link {
    font-size: 1.4rem;
    margin: 0 1.5rem;
  }

  #about .about-cards {
    flex-wrap: nowrap;
    justify-content: center;
    gap: 2rem; 
  }

  #about .about-card {
    width: 280px; 
    height: 330px; 
  }

  .dwnldbtn {
    margin-top: 2.5rem; 
  }
}

/* Tablet screens */
@media only screen and (min-width: 768px) and (max-width: 1023px) {
  .container4,
  .container5,
  .container3 {
    max-width: 650px;
    margin: 0 auto;
  }

  .profile-content {
    flex-direction: column;
    align-items: center;
    text-align: center;
  }

  .profile-info {
    max-width: 100%; 
    margin-left: 0;
  }

  .profile-image img {
    width: 100%;
    margin-left: 0;
    margin-bottom: 20px;
  }

  .cards-container {
    display: flex;
    flex-direction: column;
    gap: 4rem;
    padding: 0 50px;
  }

  .card {
    height: auto;
    width: 100%;
    max-width: 100%;
    margin: 0 auto;
  }

  .card-image {
    width: 100%;
    height: 220px;
  }

  .card-content {
    width: 100%;
    padding: 0 10px;
  }

  header .container {
    max-width: 100%;
    margin: 0 auto;
  }

  .nav-link {
    font-size: 1.3rem;
    margin: 0 1.2rem;
  }

  .card-content {
    text-align: left;
  }

  #about .about-cards {
    flex-wrap: wrap; 
    justify-content: center;
    gap: 2rem; 
  }

  #about .about-card {
    width: 250px; 
    height: auto; 
    margin-bottom: 2rem; 
  }

  .dwnldbtn {
    margin-top: 2rem; 
  }
}

/* Mobile screens */
@media only screen and (max-width: 767px) {
  .container4,
  .container2,
  .container5,
  .container3 {
    max-width: 100%;
    padding: 0 20px;
  }

  .profile-content,
  .project-content {
    flex-direction: column;
    margin-bottom: -25px;
  }

  .profile-info,
  .project-info,
  .project-image {
    max-width: 100%;
    margin: 0;
  }

  .profile-image img,
  .project-image img {
    width: 100%;
    max-width: none;
    margin-left: 0;
    margin-bottom: 45px;
    margin-top: -25px;
  }

  .card {
    flex-direction: column;
    width: 100%;
    max-width: 100%;
    height: auto;
  }

  .card-image {
    width: 100%;
    height: 200px;
    padding-right: 0;
    padding-bottom: 15px;
  }

  .card-content {
    width: 100%;
    padding: 20px 0;
  }

  .card::before, .card::after {
    display: none;
  }

  #publications h2 {
    margin-top: -90px;
  }
  
  #publications .project-headline {
    font-size: 1.4rem;
  }

  #publications .keywords {
    font-size: 0.9rem;
  }
  #publications .cardtext {
    font-size: 0.95rem;
  }
  #about .about-cards {
    flex-wrap: wrap;
    flex-direction: column; 
    align-items: center;
    gap: 1.5rem; 
  }

  #about .about-card {
    width: 90%; 
    height: auto; 
  }

  .dwnldbtn {
    margin-top: 2rem; 
  }

  #cta {
    padding: 20px;
    text-align: center;
  }

  #cta h2 {
    font-size: 1.8rem;
    margin-bottom: 15px;
  }

  #cta p {
    font-size: 1rem;
    line-height: 1.5;
    margin: 0 auto;
    max-width: 90%;
    color: #F4F4F4;
    font-family: 'Montserrat', sans-serif;
    font-weight: 400;
  }

  .contact-links {
    margin-top: 20px;
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
    gap: 15px;
  }

  .contact-item {
    font-size: 1.5rem;
  }
}
</style>

