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
  z-index: 1000; /* Set a high z-index to make sure it's above other elements */
  transition: background-color 0.3s ease; /* Add a smooth transition effect */
  background-color: #1E1E1E; /* Primary Dark Green */
  color: #c9b373; /* Light Cream */
  font-family: 'Roboto Slab', serif; /* Premium Font */
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
  text-decoration: none; /* Remove the underline */
  color: #c9b373;
  cursor: pointer; /* Change the cursor to indicate it's clickable */
  font-family: 'Roboto Slab', serif; /* Apply premium font */
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
  transition: color 0.3s ease; /* Add a smooth transition for color change */
  font-family: 'Roboto Slab', serif; /* Apply premium font */
}

.nav-link:hover {
  color: #f4f4f4;
}
</style>
