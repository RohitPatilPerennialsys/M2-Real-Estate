<template>
  <div class="instant-estimate-compo-wrapper">
    <img class="city-img" src="../assets/city.png" />
    <div class="img-content">
      <div>
        <h1>
          Do you want to know the estimate value of your property? Right Now?
        </h1>
      </div>
      <div class="instant-estimate-btn">
        <p>INSTANT ESTIMATE</p>
      </div>
    </div>
    <div class="m3-service-item-card-wrapper">
      <m3serviceitemcard
        imgsrc="../assets/Instant-Value-Estimator.png"
        itemName="Instant Value Estimator"
      ></m3serviceitemcard>
      <m3serviceitemcard
        imgsrc="../assets/registeredtrades.png"
        itemName="Registered Trades"
      ></m3serviceitemcard>
      <m3serviceitemcard
        imgsrc="../assets/constructioncostestimator.png"
        itemName="Construction Cost Estimator"
      ></m3serviceitemcard>
      <m3serviceitemcard
        imgsrc="../assets/m2ads.png"
        itemName="M2 Ads"
      ></m3serviceitemcard>
    </div>
  </div>
</template>

<script>
import m3serviceitemcard from "./m3-service-item-card.vue";
export default {
  components: {
    m3serviceitemcard,
  },
};
</script>

<style>
.m3-service-item-card-wrapper {
  display: flex;
  margin-top: 25px;
  padding-left: 25px;
  padding-right: 25px;
  flex-direction: row;
  justify-content: space-around;
  flex-wrap: wrap;
}
.img-content {
  display: flex;
  position: relative;
  justify-content: space-around;
  align-content: center;
  flex-direction: column;
  align-items: center;
}
.img-content h1 {
  padding-top: 100px;
  text-shadow: 0px 3px 7px rgba(0, 0, 0, 0.35);
  font-family: Lato;
  font-size: 20px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.6;
  letter-spacing: 1px;
  text-align: center;
  color: #fff;
}
.instant-estimate-btn p {
  margin: 0px;
  text-align: center;
  padding-top: 15px;
  font-family: Lato;
  font-size: 15px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #fff;
}
.city-img {
  opacity: 0.7;
  position: absolute;
  width: 100%;
  height: 400px;
}
.instant-estimate-btn {
  width: 143px;
  height: 50px;
  background-color: #d6ab28;
}
@media screen and (min-width: 1100px) {
  .city-img {
    height: 682px;
  }
  .img-content h1 {
    font-size: 50px;
    padding-left: 50px;
    padding-right: 50px;
  }
  .instant-estimate-btn {
    width: 250px;
    height: 65px;
  }
  .instant-estimate-btn p {
    font-size: 20px;
    padding-top: 20px;
    margin-bottom: 75px;
  }
}
</style>
