
<script>
export default {
  data() {
    return {
      isMenuOpen: false
    };
  },
  methods: {
    toggleMenu() {
      this.isMenuOpen = !this.isMenuOpen;
    }
  }
};
</script>
<template>
  <header>
      <nav class="navbar">
        <img alt="Vue logo"  src="../assets/logo.svg" width="50" height="50" />
        <div class="hamburger" @click="toggleMenu">
          <div class="bar"></div>
          <div class="bar"></div>
          <div class="bar"></div>
        </div>
        <ul :class="['nav-links', { 'active': isMenuOpen }]">
          <li><a href="#home">Home</a></li>
          <li><a href="#menu">Menu</a></li>
          <li><a href="#contact">Contact Us</a></li>
        </ul>
      </nav>
  </header>
</template>


<style scoped>
    .navbar {
      position: sticky;
      width: 100%;
      background-color: #333;
      color: white;
      padding: 20px 80px;
      display: flex;
      justify-content: space-between;
      align-items: center;
      z-index: 1000;
      box-sizing: border-box;
    }

    .nav-links {
      list-style: none;
      display: flex;
      gap: 30px;
    }

    .nav-links a {
      color: white;
      text-decoration: none;
      font-size: large;
    }

    .nav-links a:hover {
      text-decoration: underline;
      color: #f8b400;
    }

    .hamburger {
      display: none;
      flex-direction: column;
      gap: 5px;
      cursor: pointer;
    }

    .bar {
      width: 25px;
      height: 3px;
      background-color: white;
    }

    @media (max-width: 768px) {
      .hamburger {
        display: flex;
      }

      .nav-links {
        display: none;
        flex-direction: column;
        position: absolute;
        top: 60px;
        right: 0;
        background-color: #333;
        width: 100%;
        padding: 20px 20px;
        box-sizing: border-box;  
      }

      .nav-links.active {
        display: flex;
      }
    }
</style>
