<template>
  <div class="container">
    <div class="c__head">
      <div class="header">
        <div class="tdate">Tuesday, June 20</div>
        <div class="ttime">01:00 PM</div>
      </div>
      <div class="temp">
        <div class="temp__num">20°</div>
        <div class="temp__air">Northwest, 40.9km/h</div>
      </div>
    </div>
    <div class="otherland">
      <div class="ot__title">Watch other city</div>
      <div class="c__city">
        <div class="city">Belgium</div>
        <div class="city">Canada</div>
        <div class="city">France</div>
        <div class="city">Germany</div>
      </div>
    </div>
  </div>
</template>

<style scoped>
.container {
  background: var(--bg);
  height: 100%;
  padding: 5rem;
  color: #fff;
}

.c__head {
  border-bottom: 0.1rem solid #fff;
}

.header {
  display: flex;
  justify-content: space-between;
  padding: 1rem;
  font-size: 2rem;
}

.tdate {
}

.temp {
  display: flex;
  flex-direction: column;
  align-items: center;
  justify-content: center;
  padding: 5rem 2rem;
}

.temp__num {
  font-size: 10rem;
  padding-bottom: 2rem;
}

.temp__air {
  font-size: 2rem;
}

.otherland {
  padding-top: 5rem;
}

.ot__title {
  font-size: 2rem;
  padding-bottom: 2rem;
}

.c__city {
  display: flex;
  flex-direction: column;
  align-items: center;
  width: 100%;
}

.city {
  all: unset;
  width: 80%;
  height: 30px;
  font-size: 16px;
  background: transparent;
  border: none;
  position: relative;
  color: #f0f0f0;
  cursor: pointer;
  z-index: 1;
  display: flex;
  align-items: center;
  justify-content: center;
  white-space: nowrap;
  user-select: none;
  -webkit-user-select: none;
  touch-action: manipulation;
  padding: 2rem;
  font-size: 2rem;
  margin: 2rem;
}

.city::after,
.city::before {
  content: "";
  position: absolute;
  bottom: 0;
  right: 0;
  z-index: -99999;
  transition: all 0.4s;
}

.city::before {
  transform: translate(0%, 0%);
  width: 100%;
  height: 100%;
  background: #28282d;
  border-radius: 10px;
}

.city::after {
  transform: translate(10px, 10px);
  width: 35px;
  height: 35px;
  background: #ffffff15;
  backdrop-filter: blur(5px);
  -webkit-backdrop-filter: blur(5px);
  border-radius: 50px;
}

.city:hover::before {
  transform: translate(5%, 20%);
  width: 110%;
  height: 110%;
}

.city:hover::after {
  border-radius: 10px;
  transform: translate(0, 0);
  width: 100%;
  height: 100%;
}

.city:active::after {
  transition: 0s;
  transform: translate(0, 5%);
}
</style>
