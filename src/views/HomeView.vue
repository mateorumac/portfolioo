<template>
  <section id="profile">
    <div class="container4">
      <div class="profile-content">
        <div class="profile-image">
          <img src="@/assets/prof.jpg" alt="Mateo Rumac" />
        </div>
        <div class="profile-info">
          <h2 style="font-weight: bold;"><i>Mateo Rumac</i></h2>
          <p><i>Passionate Computer Science student with a strong foundation in web development.</i></p>
          <p><i> Committed to creating elegant and efficient solutions</i></p> 
        </div>
      </div>
    </div>
  </section>

  <section id="projects">
    <div class="container2">
      <h2 style="color: #fbe0c3;">My Projects</h2>
      <div class="cards-container">
        <!-- First Project Card -->
        <div class="card">
          <div class="card-image">
            <a href="https://wa-frontend-mateorumac.vercel.app/" target="_blank">
              <img src="@/assets/bba.png" alt="Beauty salon website" />
            </a>
          </div>
          <div class="card-content">
            <p>
              A beauty salon website with working backend to process user requests.<br /> <br>
              Sidenote: Backend takes a while to process requests due to inactivity and free hosting.
            </p>
          </div>
          <div class="card-footer">
            
            <a href="https://wa-frontend-mateorumac.vercel.app/" target="_blank" class="visit-link">
              <i class="fas fa-external-link-alt"></i>
            </a>
          </div>
        </div>
        <!-- Second Project Card -->
        <div class="card">
          <div class="card-image">
            <a href="https://pizzeria-jupiter-pula.onrender.com/" target="_blank">
              <img src="@/assets/pizzeria.jpg" alt="Pizzeria Jupiter" />
            </a>
          </div>
          <div class="card-content">
            <p>
              A pizza restaurant website redesigned for pizzeria Jupiter using Vue.js
            </p>
          </div>
          <div class="card-footer">
            
            <a href="https://pizzeria-jupiter-pula.onrender.com/" target="_blank" class="visit-link">
              <i class="fas fa-external-link-alt"></i>
            </a>
          </div>
        </div>
        <!-- Third Project Card -->
        <div class="card">
          <div class="card-image">
            <a href="https://stock.adobe.com/hr/search?k=work+in+progress&asset_id=101974188" target="_blank">
              <img src="@/assets/wip.jpg" alt="Work in Progress" />
            </a>
          </div>
          <div class="card-content">
            <p>
              Work in progress...
            </p>
          </div>
          <div class="card-footer">
            
            <a href="https://stock.adobe.com/hr/search?k=work+in+progress&asset_id=101974188" target="_blank" class="visit-link">
              <i class="fas fa-external-link-alt"></i>
            </a>
          </div>
        </div>
        <!-- Add more project cards as needed -->
      </div>
    </div>
  </section>

  <section id="about">
    <div class="container5">
      <h2>Some details about me</h2> <br>
      <p class="aboutme">Hello everyone!👋 <br><br> I'm Mateo Rumac, a 24-year-old computer science student based in the city of Pula, Croatia. I'm in my third year at Juraj Dobrila University, specializing in front-end web development.
      Outside of my studies, I love diving into real-world projects, transforming lines of code into meaningful digital experiences. <br><br> With a C1 proficiency in English, I handle both the technical and communication sides of projects with ease.
      Currently, I'm working on my final paper as I approach the end of my academic journey. I'm on the lookout for entry or junior-level positions in web development, eager to bring my skills and passion to new challenges. <br><br> Let's connect and turn ideas into engaging digital realities!
      If you'd like to know more about me, feel free to download my resume below!</p>
      <button class="dwnldbtn" @click="visitResumeSite">View Resume</button>
    </div>
  </section>

  <section id="cta">
    <div class="container3">
      <h2 style="color: #fbe0c3;">Ready to Start a Project?</h2>
      <p style="color: #fbe0c3;">
        Feel free to reach out to me through various channels. I'm always open to new opportunities and collaborations.
      </p>
      <div class="contact-links">
        <div class="contact-item">
          <a href="mailto:mateo.rumac@gmail.com" class="contact-item" title="Email">
            <i class="fas fa-envelope"></i>
          </a>
        </div>
        <div class="contact-item">
          <a href="https://www.facebook.com/Rooksoni21/" target="_blank" class="contact-item">
            <i class="fab fa-facebook"></i>
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
  methods: {
    visitDifferentSite() {
      const url = 'https://github.com/mateorumac/frontendWA';
      window.open(url, '_blank');
    },
    visitResumeSite() {
      const url = 'https://mateorumaccve.tiiny.site/';
      window.open(url, '_blank');
    }
  }
};
</script>

<style scoped>
h1 {
  font-size: 3rem;
  margin: 0;
  font-family: 'Roboto Slab', serif;
}

p {
  font-size: 1.25rem;
  font-family: 'Roboto Slab', serif;
}

#cta {
  background-color: #344648;
  color: #f4f4f4;
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
  font-family: 'Roboto Slab', serif;
}

.cta-button {
  display: inline-block;
  background-color: #f4f4f4;
  color: #242424;
  padding: 0.75rem 1.5rem;
  text-decoration: none;
  font-size: 1rem;
  border-radius: 5px;
  transition: background-color 0.3s, transform 0.3s ease-in-out;
  border: none; /* Remove the default border */
  outline: none;
  font-family: 'Roboto Slab', serif;
}

.cta-button:hover {
  background-color: #f4f4f4;
  transform: scale(1.05);
}

#profile {
  background-color: #fbe0c3;
  padding: 4rem 0;
}

.container4 {
  max-width: 800px;
  margin: 0 auto;
}

.profile-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.profile-image img {
  max-width: 115%;
  border-radius: 50%;
  margin-left: -60px;
}

.profile-info {
  max-width: 60%;
  margin-left: 50px;
}

.icon-padding {
  display: inline-block;
  width: 18px;
}

#projects {
  background-color: #344648;
  padding: 4rem 0;
  overflow: hidden;
  color: #f4f4f4;
}

.cards-container {
  display: flex;
  justify-content: flex-start;
  flex-wrap: wrap;
  margin-left: 15px;
}

.card {
  width: 300px;
  margin: 24px;
  border: 1px solid #ddd;
  border-radius: 8px;
  box-shadow: 0 4px 8px rgba(0, 0, 0, 0.1);
  overflow: hidden;
  display: flex;
  flex-direction: column;
  transition: transform 0.3s ease;
}

.card:hover {
  transform: scale(1.05);
}

.card-image {
  text-align: center;
}

.card-image img {
  width: 100%;
  height: 130px;
  object-fit: cover;
  border-radius: 8px 8px 0 0;
}

.card-content {
  padding: 20px;
  flex: 1;
  overflow-y: auto;
  max-height: 200px; /* Adjust this height based on your design */
}

.card-footer {
  padding: 6px;
  text-align: center;
  margin-top: auto;
}

.card-footer a {
  color: #040f13; /* Set the color of the GitHub icon */
  text-decoration: none;
  transition: color 0.3s ease;
  display: inline-block;
  padding: 0 10px;
}

.card-footer a:hover {
  color: #70abd3; /* Change color on hover */
}

#about {
  background-color: #fbe0c3;
  padding: 4rem 0;
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
  font-family: 'Roboto Slab', serif;
  display: flex;
  justify-content: center;
  align-items: center;
  flex-direction: column;
}

.dwnldbtn {
  display: inline-block;
  background-color: #344648;
  color: #fbe0c3;
  padding: 16px;
  margin-top: 10px;
  text-decoration: none;
  font-size: 1rem;
  border-radius: 5px;
  transition: background-color 0.3s, transform 0.3s ease-in-out;
  border: none; /* Remove the default border */
  outline: none;
  font-family: 'Roboto Slab', serif;
}

.dwnldbtn:hover {
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
  color: #fbe0c3;
}

.contact-item:hover {
  color: #70abd3;
}

.footer {
  position: absolute;
  bottom: 10px;
  left: 10px;
}

.footer p {
  margin: 0;
  font-size: 0.8rem; /* Smaller font size */
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
    flex-direction: row; /* Ensure content is displayed in a row */
    justify-content: space-between;
  }

  .profile-image img {
    /* Keep the profile image size unchanged */
    max-width: 115%;
    border-radius: 50%;
    margin-left: -60px;
  }

  .profile-info {
    max-width: 60%;
    margin-left: 50px;
  }

  .project-content {
    margin-left: 0;
  }

  .project-image img {
    max-width: 110%; /* Slightly smaller project images */
    border-radius: 8px;
    margin-left: 30px;
    padding: 10px;
  }

  .project-info {
    max-width: 60%; /* Allow text for projects to go a bit wider */
    padding: 20px;
    font-family: 'Roboto Slab', serif;
  }

  .container2 {
    max-width: none; /* Remove the max-width for project containers */
  }
}
/* Medium screens */
@media only screen and (max-width: 1199px) and (min-width: 768px) {
  .container4,
  .container2,
  .container5,
  .container3 {
    max-width: 600px;
  }

  .card {
    width: calc(50% - 20px); /* Adjust the width for two cards in a row */
  }
}

/* Smaller screens */
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
    margin-bottom: 20px;
  }

  .cards-container {
    margin: 0; /* Remove the negative margin for smaller screens */
  }

  .card {
    width: 100%; /* Make cards full-width on smaller screens */
  }
}
</style>
