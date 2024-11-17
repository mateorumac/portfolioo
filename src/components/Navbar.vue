<template>
  <div>
    <header>
      <div class="container">
        <router-link to="/" class="nav-link" @click="scrollToTop">
          <h1 class="nav">Mateo Rumac</h1>
        </router-link>
        <button class="hamburger" @click="toggleMenu">
          <span :class="{'open': isMenuOpen}"></span>
        </button>
        <nav class="nav-links" :class="{'mobile-menu': isMenuOpen}">
          <router-link to="#projects" class="nav-link" @click="scrollToSection('#projects'); closeMenu()">Projects</router-link>
          <router-link to="#publications" class="nav-link" @click="scrollToSection('#publications'); closeMenu()">Publications</router-link>
          <router-link to="#about" class="nav-link" @click="scrollToSection('#about'); closeMenu()">About Me</router-link>
        </nav>
      </div>
    </header>
    <router-view />
  </div>
</template>

<script>
export default {
  data() {
    return {
      isMenuOpen: false,
    };
  },
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
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
      if (this.isMenuOpen) {
        document.addEventListener('click', this.handleClickOutside);
      } else {
        document.removeEventListener('click', this.handleClickOutside);
      }
    },
    closeMenu() {
      this.isMenuOpen = false;
      document.removeEventListener('click', this.handleClickOutside);
    },
    handleClickOutside(event) {
      if (!event.target.closest('.container')) {
        this.closeMenu();
      }
    },
  },
  beforeDestroy() {
    document.removeEventListener('click', this.handleClickOutside);
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
  background-color: rgba(30, 30, 30, 0.94);
  backdrop-filter: blur(5px);
  color: #c9b373;
  font-family: 'Poppins', sans-serif;
  transition: background-color 0.3s ease, opacity 0.3s ease;
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
  color: #c9b373;
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

.hamburger {
  display: none;
  flex-direction: column;
  justify-content: space-between;
  width: 40px;
  height: 35px;
  background: transparent;
  border: none;
  cursor: pointer;
  z-index: 2000;
}

.hamburger span {
  width: 100%;
  height: 4px;
  background-color: #c9b373;
  transition: all 0.3s ease;
  position: relative;
}

.hamburger span::before,
.hamburger span::after {
  content: '';
  position: absolute;
  width: 100%;
  height: 4px;
  background-color: #c9b373;
  transition: all 0.3s ease;
}

.hamburger span::before {
  top: -10px;
}

.hamburger span::after {
  bottom: -10px;
}

.hamburger span.open {
  background-color: transparent;
}

.hamburger span.open::before {
  transform: rotate(45deg);
  top: 0;
}

.hamburger span.open::after {
  transform: rotate(-45deg);
  bottom: 0;
}

.mobile-menu {
  display: none;
  flex-direction: column;
  position: absolute;
  top: 240%;
  right: 0;
  width: 80%; 
  background-color: rgba(30, 30, 30, 0.95);
  padding: 20px;
  box-shadow: 0 10px 20px rgba(0, 0, 0, 0.3);
  z-index: 999;
  transform: translateY(-100%);
  transition: transform 0.3s ease;
}

.mobile-menu.open {
  transform: translateY(0);
}

.mobile-menu .nav-link {
  margin: 1rem 0;
  font-size: 1.4rem;
}

@media (max-width: 768px) {
  .container {
    flex-direction: row;
    justify-content: space-between;
  }

  .nav {
    text-align: left;
    margin-left: -30px;
  }

  .nav-links {
    display: none;
  }

  .nav-link::before {
    display: none;
  }
  
  .hamburger {
    display: flex;
  }

  .mobile-menu {
    display: flex;
    flex-direction: column;
  }
}

@media (min-width: 769px) {
  .nav-links {
    display: flex;
    flex-direction: row;
  }

  .mobile-menu {
    display: none;
  }

  .hamburger {
    display: none;
  }
}
</style>
