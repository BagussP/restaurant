<script setup>
import { ref, onMounted, onUnmounted } from "vue";

const showButton = ref(false);

// function buat langsung scrolling keatas
const scrollToTop = () => {
  window.scrollTo({ top: 0, behavior: "smooth" });
};

// function untuk cek kondisi apakah scrolling ada diatas atau tidak
const handleScroll = () => {
  showButton.value = window.scrollY > 0;
};

// mengaktifkan button
onMounted(() => {
  window.addEventListener("scroll", handleScroll);
});

// menonaktifkan button
onUnmounted(() => {
  window.removeEventListener("scroll", handleScroll);
});
</script>

<template>
  <button v-if="showButton" @click="scrollToTop">&#x2191;</button>
</template>

<style scoped>
button {
  position: fixed;
  bottom: 20px;
  right: 20px;
  width: 50px;
  height: 50px;
  background-color:  #f8b400;;
  color: black;
  border: none;
  border-radius: 50%;
  box-shadow: 0 4px 6px rgba(0, 0, 0, 0.1);
  cursor: pointer;
  font-size: 20px;
}

button:hover {
  background-color: #c39004;;
}
</style>
