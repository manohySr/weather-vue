<script setup>
import Landing from "@/components/Landing.vue";
import Stats from "@/components/Stats.vue";
</script>

<template>
  <div class="container__big">
    <div class="container__l">
      <div class="container__landing">
        <Landing />
      </div>
      <div class="container__stats">
        <Stats />
      </div>
    </div>
    <div class="container__r"></div>
  </div>
</template>

<style scoped>
.container__big {
  height: 100%;
  display: flex;
}

.container__l {
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  height: 100%;
  width: 75%;
  padding: 5rem;
}

.container__landing {
  height: 62%;
}

.container__stats {
  height: 35%;
}

.container__r {
  display: block;
  height: 100%;
  width: 25%;
  background: yellowgreen;
}
</style>
