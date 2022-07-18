<template>
  <div class="output-item">
    <p>{{ propertyKDVal }}</p>
  </div>
  <div class="output-item">
    <p>{{ landKDValue }}</p>
  </div>
  <div class="output-item">
    <p>{{ buildingKDValue }}</p>
  </div>
</template>

<script>
export default {
  props: ["propertyKDVal", "landKDValue", "buildingKDValue"],
};
</script>

<style>
.output-item {
  width: 292px;
  height: 66px;
  background-color: #f7f7f7;
  border-right: 1px solid #032149;
}
.output-item p {
  margin-top: 13px;
  font-family: Lato;
  font-size: 26px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.69;
  letter-spacing: normal;
  text-align: center;
  color: #4a6084;
}
</style>
