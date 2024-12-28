<template>
  <section id="contact">
    <h3>Contact Us</h3>
    <p>Email: info@deliciousbites.com</p>
    <p>Phone: +1-800-555-1234</p>
    <p>Follow us:</p>
    <div class="social">
      <a href="#">Facebook</a>
      <a href="#">Instagram</a>
      <a href="#">Twitter</a>
    </div>
  </section>
</template>

<style scoped>
section#contact {
  background-color: #333;
  color: white;
  padding: 20px;
  text-align: center;
}

h3 {
  margin-bottom: 10px;
  font-size: 1.8em;
}

p {
  margin: 5px 0;
}

.social {
  margin-top: 10px;
}

.social a {
  margin: 0 10px;
  color: #f8b400;
  text-decoration: none;
  transition: color 0.3s;
}

.social a:hover {
  color: white;
  text-decoration: underline;
}
</style>
