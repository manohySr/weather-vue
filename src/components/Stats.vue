<template>
  <div class="container">
    <span class="title">Today's statistics</span>
    <div class="container__siweather">
      <div class="siweather" v-for="n in 5">
        <div class="siweather__number">27°</div>
        <div class="siweather__time">09:00 AM</div>
        <div class="siweather__description">Sunny cloudy</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  border-radius: 2rem;
  padding: 2rem 5rem;
  background: rgba(42, 43, 47, 255);
  color: aliceblue;
  width: 100%;
}

.container__siweather {
  display: flex;
  justify-content: center;
  gap: 2rem;
}

.title {
  font-size: 2rem;
}

.siweather {
  margin-top: 2rem;
  display: block;
  padding: 2rem 0;
  width: 19%;
  background-color: red;
}

.siweather__number {
  display: flex;
  justify-content: center;
  padding: 0 2rem 2rem 2rem;
  font-size: 5rem;
}

.siweather__time {
  display: flex;
  justify-content: center;
  font-size: 1.8rem;
  padding-bottom: 1rem;
}

.siweather__description {
  display: flex;
  justify-content: center;
  font-size: 1.8rem;
  padding-bottom: 1rem;
}
</style>
