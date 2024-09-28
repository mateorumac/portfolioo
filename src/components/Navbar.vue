<template>
  <div>
    <header>
      <div class="container">
        <router-link to="/" class="nav-link" @click="scrollToTop">
          <h1 class="nav">Mateo Rumac</h1>
        </router-link>
        <nav class="nav-links">
          <router-link to="#projects" class="nav-link" @click="scrollToSection('#projects')">My Projects</router-link>
          <router-link to="#about" class="nav-link" @click="scrollToSection('#about')">About Me</router-link>
        </nav>
      </div>
    </header>
    <router-view />
  </div>
</template>

<script>
export default {
  methods: {
    scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: "smooth",
      });
    },
    scrollToSection(sectionId) {
      const section = document.querySelector(sectionId);
      if (section) {
        section.scrollIntoView({
          behavior: "smooth",
        });
      }
    },
  },
};
</script>

<style scoped>
header {
  position: sticky;
  top: 0;
  padding: 28px;
  width: 100%;
  z-index: 1000;
  transition: background-color 0.3s ease, opacity 0.3s ease;
  background-color: rgba(30, 30, 30, 0.94); 
  backdrop-filter: blur(5px); 
  color: #c9b373;
  font-family: 'Poppins', sans-serif;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
}

.nav {
  font-size: 2.3rem; 
  font-weight: 700; 
  letter-spacing: 0.05em; 
  color: #f4f4f4; 
  text-transform: uppercase;
  margin: 0;
  text-decoration: none;
  cursor: pointer;
  transition: transform 0.3s ease;
  
}

.nav:hover {
  transform: scale(1.05); 
}

.nav-links {
  display: flex;
  align-items: center;
}

.nav-link {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: #f4f4f4;
  margin: 0 1rem;
  font-size: 1.3rem;
  cursor: pointer;
  transition: transform 0.3s ease, background-position 0.3s ease;
  font-family: 'Poppins', sans-serif;
  position: relative;
}

.nav-link::before {
  content: '';
  position: absolute;
  width: 0;
  height: 2px;
  bottom: 0;
  left: 0;
  background-color: #c9b373;
  visibility: hidden;
  transition: width 0.3s ease-in-out;
}

.nav-link:hover::before {
  visibility: visible;
  width: 100%; 
}

.nav-link:hover {
  transform: scale(1.1); 
}

/* Media query for mobile view */
@media (max-width: 768px) {
  .container {
    flex-direction: row;
    justify-content: space-between;
  }

  .nav {
    flex: 1;
    text-align: left;
    margin-left: -26px;
  }

  .nav-links {
    flex: 1;
    justify-content: flex-end;
    margin-left: 0.9rem;
    margin-right: -1.2rem;
  }

  .nav-link {
    margin: 0 0.5rem;
    font-size: 1.2rem;
  }
}
</style>
