<template>
  <div class="card-item-wrapper">
    <img class="service-card-image" :src="imgsrc" alt="" />
    <p class="service-card-name">{{ itemName }}</p>
  </div>
</template>

<script>
export default {
  props: ["imgsrc", "itemName"],
};
</script>

<style>
.card-item-wrapper {
  display: flex;
  flex-direction: column;
  justify-content: center;
  align-items: center;
  margin: 20px 20px 0px 20px;
  width: 300px;
  height: 300px;
  border-radius: 6px;
  background-color: #4a6084;
  z-index: 1;
}
.service-card-image {
  width: 100px;
  height: 100px;
}
.service-card-name {
  font-family: Lato;
  font-size: 25.5px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: center;
  color: #fff;
}
</style>
