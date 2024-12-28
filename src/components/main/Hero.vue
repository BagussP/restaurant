<template>
  <section class="hero">
    <div class="hero-text">
      <h1>Welcome to Delicious Bites</h1>
      <p>Fresh Ingredients. Tasty Meals. Unforgettable Experiences.</p>
    </div>
    <img src="../../assets/hero.png" alt="steak" width="500" height="" />
    <!-- <img src="../../assets/background-hero.jpg" class="background" alt="steak" width="3000" height="" /> -->
  </section>
</template>

<style scoped>
.hero {
  position: relative;
  background: url("../../assets/background-hero.png") no-repeat center
    center/cover;
  height: 100vh;
  display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 0px 80px;
  color: white;
  font-size: 28px;
}

@media (max-width: 1024px) {
  img {
    width: 300px;
  }
}

@media (max-width: 768px) {
  .hero {
    flex-direction: column-reverse;
    justify-content: center;
    align-items: center;
    text-align: center;
    font-size: 20px;
  }

  img {
    width: 300px;
  }
}
</style>
