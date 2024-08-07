<template>
  <div>
    <header>
      <div class="container">
        <router-link to="/" class="nav-link" @click="scrollToTop">
          <h1 class="nav">Mateo Rumac</h1>
        </router-link>
        <nav class="nav-links">
          <router-link to="#projects" class="nav-link" @click="scrollToSection('#projects')">Projects</router-link>
          <router-link to="#about" class="nav-link" @click="scrollToSection('#about')">About</router-link>
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
  padding: 23px;
  width: 100%;
  z-index: 1000;
  transition: background-color 0.3s ease;
  background-color: #1E1E1E;
  color: #c9b373;
  font-family: 'Roboto Slab', serif;
}

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
}

.nav {
  font-size: 2rem;
  margin: 0;
  text-decoration: none;
  color: #c9b373;
  cursor: pointer;
  font-family: 'Roboto Slab', serif;
}

.nav:hover {
  color: #f4f4f4;
}

.nav-links {
  display: flex;
  align-items: center;
}

.nav-link {
  display: flex;
  align-items: center;
  text-decoration: none;
  color: #c9b373;
  margin: 0 1rem;
  font-size: 1.3rem;
  cursor: pointer;
  transition: color 0.3s ease;
  font-family: 'Roboto Slab', serif;
}

.nav-link:hover {
  color: #f4f4f4;
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
