<!-- hero section -->

<script setup>
import HeroAnimation from "@/animations/HeroAnimation";
import { onMounted } from "vue";
import rightArrow from "@/assets/svgs/rightArrow.vue";
import FirstTransitionAnimation from "@/animations/FirstTransitionAnimation";

onMounted(() => {
  HeroAnimation();
});
</script>

<template>
  <section id="section-1" class="skew-container">
    <div class="w-100 h-100 skew">
      <div
        class="h-100 d-flex flex-column justify-content-center titles-container"
      >
        <h1 class="hero-title-1">Matías Berríos</h1>
        <h1 class="hero-title-2">Desarrollador y estudiante chileno</h1>
        <div class="hero-title-3">
          > especialista en: &nbsp;
          <div id="typewriter"></div>
        </div>
      </div>
    </div>
    <rightArrow class="right-arrow" @click="FirstTransitionAnimation()" />
  </section>
</template>
