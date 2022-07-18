<template>
  <div class="marquee-container">
    <div class="strip-date-month">
      19 Sep<span class="strip-date-year"><br />2016</span>
    </div>
    <div class="verticalLine">|</div>
    <marquee class="marquee-wrapper" direction="left">
      <span class="strip-content">
        <span class="bold">SALE</span>: Kaifan, Land ,500sqm, 20 Sep 2016</span
      >

      <span class="strip-content">
        | <span class="bold">WANTED</span>: Nuzha, House, 750sqm, 21 Sep 2016 |
        RENT: Faiha, Flat, 3 BR, 21 Sep 2016
      </span>
      <span class="strip-content">
        |<span class="bold">RENT</span> : Faiha, Flat, 3 BR, 21 Sep 2016
      </span>
    </marquee>
  </div>
</template>

<script>
export default {};
</script>

<style>
.marquee-container {
  display: flex;
  background-color: #d6ab28;
  height: 51px;
}
.bold {
  font-weight: bold;
}
.strip-date-month {
  height: 29px;
  font-family: Lato;
  font-size: 16px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: 1px;
  text-align: left;
  color: #fff;
  padding: 6px 0px 11px 15px;
}
.strip-date-year {
  font-size: 15px;
  letter-spacing: 5.7px;
}
.verticalLine {
  font-size: 30px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  text-align: left;
  color: #fff;
  padding-top: 6px;
  padding-left: 10px;
}
.marquee-wrapper {
  font-family: Lato;
  font-size: 16px;
  padding-top: 10px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.88;
  letter-spacing: 2px;
  text-align: left;
  color: #fff;
}
.strip-content {
  padding-left: 30px;
}
@media screen and (min-width: 1100px) {
  .marquee-container {
    padding-left: 284px;
  }
}
</style>
