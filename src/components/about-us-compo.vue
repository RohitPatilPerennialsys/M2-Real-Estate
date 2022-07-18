<template>
  <div class="about-us-wrapper">
    <div class="footer-logo">
      <img src="../assets/logofooter.png" alt="" />
    </div>
    <div class="about-us-item-wrapper">
      <div class="about-us-item-contact">
        <p>CONTACT</p>
        <div class="about-us-item">
          <p>
            Office: realestate.com No. 12, Real Estae Building, Real Estate
            street, Kuwait.
            <br />
            Call Us: +965 0000 0000 +965 0000 0000
          </p>
        </div>
      </div>
      <div class="about-us-item-my-account">
        <p>MY ACCOUNT</p>
        <div class="about-us-item">
          <p>
            Create new account <br />
            Login
          </p>
        </div>
      </div>
      <div class="about-us-item-lasted-news">
        <p>LASTED NEWS</p>
        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.Lorem ipsum
          dolor sit amet, consectetur adipisicing elit.<br />
          ------------------------------------<br /><br /><br />
          Lorem ipsum dolor sit amet, consectetur adipisicing elit.Lorem ipsum
          dolor sit amet, consectetur adipisicing elit.<br />
          ------------------------------------<br />
        </p>
      </div>
      <div class="about-us-item-newsletter-signup">
        <p>NEWSLETTER SIGNUP</p>
        <p>Subscribe to Our Newsletter to get the latest about M2:</p>
        <div class="input-field-wrapper">
          <input class="input-field" /><br /><br />
          <input class="submit-btn" type="submit" value="Submit" />
        </div>
        <div class="connect-with-us-wrapper">
          <p class="connect-with-us-title">CONNECT WITH US</p>
          <div class="social-media">
            <img src="../assets/footer-twitter.png" alt="" />
            <img
              class="social-media-img"
              src="../assets/footer-instagram.png"
              alt=""
            />
            <img
              class="social-media-img"
              src="../assets/footer-google.png"
              alt=""
            />
            <img
              class="social-media-img"
              src="../assets/footer-facebook.png"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {};
</script>

<style>
/*  */
.social-media-img {
  padding-left: 25px;
}
.social-media {
  display: flex;
}
.connect-with-us-title {
  font-family: Lato;
  font-size: 24px;
  margin-bottom: 0px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #4a525d;
}
/*  */
.input-field-wrapper {
  display: flex;
  flex-direction: row;
}
.input-field {
  width: 202px;
  height: 38px;

  border: solid 1px #2e3338;
  background-color: #161616;
}
.submit-btn {
  width: 76px;
  height: 38px;
  border: solid 1px #2e3338;
  background-color: #161616;
  margin-left: 10px;
  margin-top: 2px;
}
input[type="submit" i] {
  font-family: Raleway;
  font-size: 14px;
  padding: 0px;
  font-weight: normal;
  font-stretch: normal;
  font-style: normal;
  line-height: 2.14;
  letter-spacing: normal;
  text-align: center;
  color: #fff;
}
/*  */
.footer-logo {
  display: flex;
  justify-content: center;
  margin-bottom: 50px;
}
.about-us-wrapper {
  background-color: #161616;
}
.about-us-wrapper img {
  margin-top: 25px;
}
.about-us-item-wrapper {
  flex-direction: row;
  justify-content: space-between;
  display: flex;
  flex-wrap: wrap;
  margin-left: 34px;
  margin-right: 34px;
  padding-bottom: 30px;
}
.about-us-item-contact {
  width: 188px;
}
.about-us-item-lasted-news {
  width: 300px;
}
.about-us-item-my-account {
  width: 200px;
}
.about-us-item-newsletter-signup {
  width: 300px;
}
.about-us-item-contact p,
.about-us-item-lasted-news p,
.about-us-item-my-account p,
.about-us-item-newsletter-signup p {
  font-family: Lato;
  font-size: 22px;
  font-weight: bold;
  font-stretch: normal;
  font-style: normal;
  line-height: normal;
  letter-spacing: normal;
  text-align: left;
  color: #4a525d;
}
</style>
