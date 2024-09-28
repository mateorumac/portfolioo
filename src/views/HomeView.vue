<template>
  <section id="profile">
    <div class="container4">
      <div class="profile-content">
        <div class="profile-image">
          <img src="@/assets/prof1.jpg" alt="Mateo Rumac" />
        </div>
        <div class="profile-info">
          <h2 >Mateo Rumac</h2>
          <p class="subtext"><i>Univ. Bacc. Inf. </i></p> <br>
          <p class="description">Passionate developer with a strong foundation in web <br> frontend development.</p> <br>
          <p class="description">Committed to creating elegant and efficient solutions</p> 
        </div>
      </div>
    </div>
  </section>

  <section id="projects">
    <div class="container2">
      <h2>My Projects</h2>
      <div class="cards-container">
        <div class="card">
          <div class="card-image">
            <a href="https://bbuddy-mateorumacs-projects.vercel.app/" target="_blank">
              <img src="@/assets/bbuddy.jpg" alt="Work in Progress" />
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
        <div class="card">
          <div class="card-image">
            <a href="https://portfoliotemplate-mateorumacs-projects.vercel.app/" target="_blank">
              <img src="@/assets/portfolioheader.png" alt="Portfolio website template" />
            </a>
          </div>
          <div class="card-content">
            <h3 class="project-headline">Portfolio template</h3>
            <p class="cardtext">
              A sleek and responsive portfolio website template, crafted with precision using HTML and CSS, designed to showcase work with a clean and modern aesthetic.
            </p>
          </div>
        </div>
        
        <!-- Add more cards -->
      </div>
    </div>
  </section>
  <section id="about">
    <div class="container5">
      <h2>Some details about me</h2> <br>
      <p class="aboutme">Hello everyone!👋 <br><br> I'm Mateo Rumac, a 24-year-old recent graduate from Juraj Dobrila University in Pula, Croatia, specializing in front-end web development. Outside of my academic journey, I love diving into real-world projects, transforming lines of code into meaningful digital experiences.
        <br><br><br>With a C1 proficiency in English, I handle both the technical and communication sides of projects with ease. I'm on the lookout for entry or junior-level positions in web development, eager to bring my skills and passion to new challenges.
        <br><br><br>Let's connect and turn ideas into engaging digital realities! If you'd like to know more about me, feel free to download my resume below!</p><br>
      <button class="dwnldbtn" @click="visitResumeSite">View Resume</button>
    </div>
  </section>
  <section id="cta">
    <div class="container3">
      <h2>Ready to Start a Project?</h2>
      <p>
        Feel free to reach out to me through various channels. I'm always open to new opportunities and collaborations.
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
  methods: {
    visitDifferentSite() {
      const url = 'https://github.com/mateorumac/frontendWA';
      window.open(url, '_blank');
    },
    visitResumeSite() {
      const url = 'https://mateorumaccveng.tiiny.site/';
      window.open(url, '_blank');
    }
  }
};
</script>

<style scoped>
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@400;700&display=swap');


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
  max-width: 800px;
  margin: 0 auto;
}

.profile-content {
  display: flex;
  justify-content: space-between;
  align-items: center;
}

.profile-image img {
  width: 125%; 
  border-radius: 15px; 
  box-shadow: 0 8px 16px rgba(0, 0, 0, 0.3); 
  margin-left: -200px; 
  transition: transform 0.3s ease, box-shadow 0.3s ease; 
}

.profile-image img:hover {
  transform: scale(1.05); 
  box-shadow: 0 12px 24px rgba(0, 0, 0, 0.3);
}

.profile-info {
  max-width: 80%; 
  margin-left: 40px; 
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

#about {
  background-color: #2c2c2c; 
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

  .dwnldbtn {
    font-size: 1.2rem;
    padding: 14px 20px;
  }

  header .container {
    max-width: 1200px;
    margin: 0 auto;
  }

  .nav-link {
    font-size: 1.4rem;
    margin: 0 1.5rem;
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

  .dwnldbtn {
    font-size: 1.1rem;
    padding: 12px 16px;
  }

  header .container {
    max-width: 100%;
    margin: 0 auto;
  }

  .nav-link {
    font-size: 1.3rem;
    margin: 0 1.2rem;
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
}
</style>