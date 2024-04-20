<template>
  <div>
    <header> 
      <div class="container">
        <router-link to="/" class="nav-link" @click="scrollToTop"><h1 class="nav">Mateo Rumac</h1>
        </router-link>
        <nav class="nav-links">
          <router-link to="#projects" class="nav-link" @click="scrollToSection('#projects')">Projects</router-link>
          <router-link to="#about" class="nav-link" @click="scrollToSection('#about')">About me</router-link>    
          
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
  color: #ffffff;
  padding: 10px;
  width: 100%;
  z-index: 1000; /* Set a high z-index to make sure it's above other elements */
  transition: background-color 0.3s ease; /* Add a smooth transition effect */
  background-color: #344648;
  color: #fbe0c3;
  padding: 23px;
  font-family: 'Roboto Slab', serif;
  }

.container {
  display: flex;
  justify-content: space-between;
  align-items: center;
  box-sizing: border-box;
}
.nav:hover {
  color: #70abd3; /* Change the color on hover */
}
.nav {
  font-size: 2rem;
  margin: 0;
  text-decoration: none; /* Remove the underline */
  color: #fbe0c3; /* Set the default text color */
  cursor: pointer; /* Change the cursor to indicate it's clickable */
}

.nav-links {
    display: flex;
    align-items: center;
  }
.nav-link {
  display: flex;
    align-items: center;
  text-decoration: none;
  color: #fbe0c3;
  margin: 0 1rem;
  font-size: 1rem;
  cursor: pointer;
  transition: color 0.3s ease; /* Add a smooth transition for color change */
}

.nav-link:hover {
  color: #70abd3; /* Change the color on hover */
}

</style>
