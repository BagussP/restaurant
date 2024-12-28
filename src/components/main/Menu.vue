<template>
  <section id="menu" class="featured">
    <h2>Popular Dishes</h2>
    <div class="dishes">
      <div class="dish">
        <img
          src="../../assets/spaghetti.jpg"
          width="280"
          height="280"
          alt="Spaghetti Carbonara"
        />
        <h3>Spaghetti Carbonara</h3>
        <p>Classic Italian pasta with creamy sauce and pancetta.</p>
      </div>
      <div class="dish">
        <img
          src="../../assets/steak.jpg"
          width="280"
          height="280"
          alt="Grilled Steak"
        />
        <h3>Grilled Steak</h3>
        <p>Perfectly grilled steak served with mashed potatoes.</p>
      </div>
      <div class="dish">
        <img
          src="../../assets/salad.jpg"
          width="280"
          height="280"
          alt="Caesar Salad"
        />
        <h3>Caesar Salad</h3>
        <p>Fresh greens tossed in Caesar dressing with croutons.</p>
      </div>
    </div>
  </section>
</template>

<style scoped>
#menu {
  box-sizing: border-box;
  /* height: 100vh; */
  padding: 100px 0px;
}

h2{ 
    text-align: center;
    margin-bottom: 50px;
    font-size: 30px;
}

.dishes {
  display: flex;
  width: 100%;
  box-sizing: border-box;
  padding: 0 80px;
  justify-content: space-evenly;
}

.dish {
    background-color: white ;
    width: 280px;
    height: 400px;
    border-radius: 20px;
    display: flex;
    flex-direction: column;
    align-items: center ;
    box-shadow: 0px 0px 13px 0px rgba(0, 0, 0, 0.3);
    transition: 300ms;
}

.dish:hover {
  margin-top: -10px;
    box-shadow: 0px 0px 20px 1px rgba(0, 0, 0, 1);

}

img {
    border-radius:20px 20px 0px 0px;
    height: 220px;
    object-fit: cover;
}

p {
    width: 230px;
}

@media (max-width: 1024px) {
  .dishes {
    flex-direction: column;
    align-items: center;
  }

  .dish {
    margin-bottom: 20px;
  }
}
</style>
