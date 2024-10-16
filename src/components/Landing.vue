<template>
  <div class="container" style="color: aliceblue">
    <div class="location">
      <i class="pi pi-map-marker" style="font-size: 3rem"></i>
      <span class="location__title">Purwokerto, Barnyumas</span>
    </div>
    <div>
      <span class="weather__static">Weather Forecast</span>
      <div class="weather">
        <span class="weather__dynamic">Overcast cloudy</span>
        <span class="weather__description"
          >The low temperature will reach 25° on this gloomy day
        </span>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  height: 100%;

  background-image: linear-gradient(rgba(0, 0, 0, 0.2), rgba(0, 0, 0, 0.5)),
    url("@/assets/sunny.png");
  background-size: cover;
  background-attachment: fixed;
  background-position-x: right;
  background-position-y: bottom;
  padding: 5rem;
  display: flex;
  flex-direction: column;
  justify-content: space-between;
  border-radius: 2rem;
}

.location {
  display: flex;
  align-items: center;
  gap: 1rem;
}

.location__title {
  font-size: 3.5rem;
}

.weather__static {
  font-size: 2rem;
  display: block;
  padding-bottom: 3rem;
}

.weather {
  display: flex;
  flex-direction: column;
}

.weather__dynamic {
  font-size: 8rem;
}

.weather__description {
  display: block;
  padding-top: 0.5rem;
  font-size: 2.1rem;
}
</style>
