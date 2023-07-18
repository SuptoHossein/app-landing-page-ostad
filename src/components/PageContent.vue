<template>
  <div class="page-content">
    <div>
    <!-- Features Component -->
      <div class="container">
        <Features />
      </div>

      <!-- Divider Component -->
      <Divider />

      <!-- About Component -->
      <About />

      <!-- Screenshot Component -->
      <Screenshot />

      <!-- Price Component -->
      <Price />

      <!-- Divider Component -->
      <Divider />

      <!-- Testimonial Component -->
      <Testimonial />

      <!-- Download Component -->
      <Download />
    </div>
  </div>
</template>

<script setup>
import Features from './Features.vue'
import About from './About.vue'
import Screenshot from "./Screenshot.vue";
import Price from "./Price.vue";
import Testimonial from "./Testimonial.vue";
import Download from "./Download.vue";
import Divider from "./Divider.vue";
</script>