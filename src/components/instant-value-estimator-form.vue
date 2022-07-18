<template>
  <div class="instant-value-estimator-form-wrapper">
    <h1 class="instant-value-estimator-form-heading">
      Instant Value Estimator
    </h1>
    <!--  -->
    <div class="instant-value-estimator-form">
      <instantvalueformitemwrapper
        labeltitle="Area"
        labelvalue="Area Name"
      ></instantvalueformitemwrapper>

      <form class="form-item">
        <label class="item-title">Land Size (Sqm)</label>
        <input class="select" value="250" />
      </form>

      <instantvalueformitemwrapper
        labeltitle="Street Type"
        labelvalue="Street type name"
      ></instantvalueformitemwrapper>

      <instantvalueformitemwrapper
        labeltitle="Plot Location"
        labelvalue="Back Plot"
      ></instantvalueformitemwrapper>

      <form class="form-item">
        <label class="item-title">Back front length</label>
        <input class="select" value="30" />
      </form>
    </div>
    <!--  -->
    <div class="radio-wrapper">
      <h1>Property type</h1>
      <label class="radio-label"
        ><p>Land</p>
        <input class="radio-btn-input" type="radio" name="radio" />
        <span class="custom-radio-button"></span>
      </label>
      <label class="radio-label"
        ><p>House</p>
        <input class="radio-btn-input" type="radio" name="radio" />
        <span class="custom-radio-button"></span>
      </label>
    </div>

    <!--  -->
    <div class="instant-value-estimator-form">
      <instantvalueformitemwrapper
        labeltitle="Property Status"
        labelvalue="Developed Building"
      ></instantvalueformitemwrapper>
      <instantvalueformitemwrapper
        labeltitle="House Age (years)"
        labelvalue="1-5"
      ></instantvalueformitemwrapper>
      <instantvalueformitemwrapper
        labeltitle="Finishing Quality"
        labelvalue="Luxurious"
      ></instantvalueformitemwrapper>
      <instantvalueformitemwrapper
        labeltitle="Basement"
        labelvalue="Luxurious"
      ></instantvalueformitemwrapper>
      <instantvalueformitemwrapper
        labeltitle="No. of Floors"
        labelvalue="1"
      ></instantvalueformitemwrapper>
      <instantvalueformitemwrapper
        labeltitle="Specification List 1"
        labelvalue="Specification Name"
      ></instantvalueformitemwrapper>
    </div>
    <!--  -->
    <div class="advance-search-wrapper">
      <img src="../assets/advanced-search.png" />
      <p>Advanced Search</p>
    </div>
    <!--  -->
    <div class="calculate-wrapper">
      <div class="calculate-container">
        <p>CALCULATE</p>
      </div>
    </div>
    <!--  -->
    <p class="output-heading-title">Output</p>
    <div class="final">
      <div class="output-container">
        <div class="output-wrapper">
          <div class="output-item-container">
            <p>Property (KD)</p>
          </div>
          <div class="output-item-container-land">
            <p>Land (KD)</p>
          </div>
          <div class="output-item-container">
            <p>Building (KD)</p>
          </div>
        </div>
        <div class="output-wrapper">
          <outputitem
            propertyKDVal="1,702,500"
            landKDValue="943,000"
            buildingKDValue="759,500"
          ></outputitem>
        </div>
      </div>
      <div class="social-media-wrapper">
        <p class="social-media-heading">Share with</p>
        <div class="social-media-item-container">
          <div class="social-media-item">
            <img src="../assets/twitter-logo-blue.png" alt="" />
          </div>
          <div class="social-media-item">
            <img src="../assets/facebook-logo.png" alt="" />
          </div>
          <div class="social-media-item">
            <img src="../assets/outbook-logo.png" alt="" />
          </div>
          <div class="social-media-item">
            <img src="../assets/instagram-logo.png" alt="" />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
import instantvalueformitemwrapper from "./instant-value-form-item-wrapper.vue";
import outputitem from "./output-item.vue";
export default {
  components: {
    instantvalueformitemwrapper,
    outputitem,
  },
};
</script>

<style>
/*  */

/*  */
.advance-search-wrapper {
  display: flex;
  margin-top: 20px;
  flex-direction: row;
  justify-content: center;
  align-items: center;
}
.advance-search-wrapper p {
  width: 250px;
  margin: 0px;
  padding-left: 20px;
  font-family: roboto;
  font-size: 20px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.5;
  letter-spacing: normal;
  text-align: left;
  color: #fff;
}
/*  */
.radio-label p {
  padding-top: 3px;
  margin: 0;
}
.instant-value-estimator-form {
  display: flex;
  flex-direction: row;
  justify-content: center;
  flex-wrap: wrap;
}

/*  */
.instant-value-estimator-form-wrapper {
  background-color: #4a6084;
  margin-top: 25px;
}
.instant-value-estimator-form-heading {
  display: flex;
  margin-bottom: 25px;
  padding-top: 30px;
  align-items: center;
  justify-content: center;
  font-family: Lato;
  font-size: 25px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.67;
  letter-spacing: normal;
  text-align: center;
  color: #fff;
}
.radio-wrapper {
  display: flex;
  flex-direction: row;
  justify-content: center;
}
.radio-wrapper h1 {
  font-family: Roboto;
  margin-top: 0px;
  padding-top: 18px;
  margin-right: 10px;
  margin-left: 35px;
  font-size: 18px;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.75;
  letter-spacing: normal;
  text-align: left;
  color: #fffefe;
}
/* radio button  */
.radio-label {
  display: block;
  position: relative;
  padding-right: 30px;
  padding-left: 35px;
  margin: 12px 0;
  cursor: pointer;
  font-size: 18px;
  font-family: Roboto;
  font-weight: 500;
  font-stretch: normal;
  font-style: normal;
  line-height: 1;
  letter-spacing: normal;
  text-align: left;
  color: #fffefe;
}

/* Hide the default radio button */
.radio-btn-input {
  position: absolute;
  opacity: 0;
  cursor: pointer;
}

/* Creating own radio button to style */
.custom-radio-button {
  position: absolute;
  top: 0;
  left: 0;
  height: 24px;
  width: 24px;
  background-color: #eee;
  border-radius: 50%;
}

/* button checked */
label input:checked + .custom-radio-button {
  background-color: #d6ab28;
}
/*  */
.calculate-wrapper {
  display: flex;
  justify-content: space-around;
  margin-top: 35px;
}

.calculate-container {
  width: 184px;
  height: 50px;
  background-color: #032149;
}
.calculate-container p {
  font-family: lato;
  margin: 0%;
  padding-top: 10px;
  text-align: center;
  font-size: 16px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.88;
  letter-spacing: normal;
  color: #fff;
}
/*  */
.output-heading-title {
  display: flex;
  justify-content: center;
  font-family: Lato;
  font-size: 20px;
  margin: 0px;
  padding-bottom: 20px;
  padding-top: 35px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 0.67;
  letter-spacing: normal;
  text-align: center;
  color: #fff;
}
/*  */
.output-wrapper {
  justify-content: center;
  display: flex;
  flex-direction: row;
  margin-left: 10px;
  margin-right: 10px;
}
.output-item-container {
  display: flex;
  flex-direction: column;
  width: 292px;
  height: 88px;
  background-color: #032149;
  margin-top: 14px;
}
.output-item-container p,
.output-item-container-land p {
  font-family: Lato;
  font-size: 20px;
  margin-top: 30px;
  margin-bottom: 0px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.83;
  letter-spacing: normal;
  text-align: center;
  color: #fff;
}

.output-item-container-land {
  width: 292px;
  height: 102px;
  background-color: #d6ab28;
}
/*  */
.social-media-item-container {
  display: flex;
  flex-direction: row;
}
.social-media-wrapper {
  display: flex;
  flex-direction: column;
  align-items: center;
  padding-bottom: 100px;
}
.social-media-item {
  width: 50px;
  height: 50px;
  margin-left: 20px;
  background-color: #fff;
  border-radius: 50%;
}
.social-media-heading {
  font-family: Lato;
  font-size: 18px;
  margin-top: 35px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: 1.67;
  letter-spacing: normal;
  text-align: left;
  color: #fff;
}
.social-media-item img {
  padding: 12px 0px 0px 12px;
}
@media screen and (min-width: 1100px) {
  .instant-value-estimator-form-heading {
    justify-content: flex-start;
    padding-left: 15px;
  }
  .instant-value-estimator-form-wrapper {
    padding-left: 25px;
  }
  .instant-value-estimator-form {
    display: flex;
    flex-direction: row;
    justify-content: flex-start;
    flex-wrap: wrap;
  }
  .radio-wrapper {
    justify-content: flex-start;
  }
  .radio-wrapper h1 {
    margin-left: 15px;
  }
  .advance-search-wrapper {
    justify-content: flex-start;
    margin-left: 15px;
  }
  .calculate-wrapper {
    margin-right: 55px;
    justify-content: flex-end;
  }
  .output-heading-title {
    padding-left: 15px;
    justify-content: flex-start;
  }
  .output-wrapper {
    justify-content: flex-start;
  }
}
@media screen and (min-width: 1275px) {
  .final {
    display: flex;
  }
  .social-media-wrapper {
    align-items: flex-start;
  }
  .social-media-heading {
    margin-left: 70px;
  }
  .social-media-item-container {
    margin-left: 50px;
  }
}
</style>
