<template>
  <div>
    <div class="main" id="contacts">
      <div class="text">
        <div class="title">Contact with our team</div>
        <p>If you are planning on developing a product landing.</p>
      </div>

      <div class="contact-info">
        <div class="left-side">
          <div class="map">
            <img
              class="map-img"
              src="../../assets/img/StaticMapService.GetMapIma.png"
              alt=""
            />

            <div class="indicazioni c-pointer">
              <div class="left-part">
                <div>Storey Ave</div>
                <div>San Francisco, California 94129</div>
                <div>Visualizza mappa più grande</div>
              </div>
              <div class="right-part">
                <img src="../../assets/img/indicazioni.png" alt="" />
                <div>Indicazi...</div>
              </div>
            </div>

            <div class="zoom c-pointer">
              <i class="fas fa-plus"></i>
              <div class="line"></div>
              <i class="fas fa-minus"></i>
            </div>

            <div class="location">
              <img src="../../assets/img/pointmap.png" alt="" />
            </div>

            <div class="legal-info c-pointer">
              <div>Dati mappa ©2020</div>
              <div>Termini e condizioni d'uso</div>
              <div>Segnala un errore nella mappa</div>
            </div>

            <div class="place-img">
              <img src="../../assets/img/mountain.jpg" alt="" />
            </div>
          </div>
        </div>

        <div class="right-side">
          <img class="logo" src="../../assets/img/35.png" alt="" />

          <div class="street">9840 Shore St. Fond Du Lac, WI 54935</div>

          <div class="contacts">
            <div>0 1223 456 789</div>
            <div>mail@sofbox.com</div>
          </div>

          <div class="social">
            <div
              class="icon-cont c-pointer"
              v-for="(social, index) in social"
              :key="index"
            >
              <i :class="social"></i>
            </div>
          </div>

          <div class="input-section">
            <div class="subtitle">Get in Touch</div>

            <div class="personal-info">
              <input type="text" placeholder="Your Name" />
              <input type="text" placeholder="Your Email" />
            </div>

            <div class="subject">
              <input type="text" placeholder="Your Subject" />
            </div>

            <div class="user-message">
              <textarea
                name="message"
                id="contact-msg"
                cols="30"
                rows="10"
                placeholder="Your Message"
              ></textarea>
            </div>
          </div>

          <button class="general-btn">Send Message</button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      social: [
        "fa-brands fa-facebook-f",
        "fa-brands fa-twitter",
        "fa-brands fa-github",
        "fa-brands fa-instagram",
      ],
    };
  },
};
</script>

<style lang="scss" scoped>
@import "@/style/MainS-Components/ContactSection.scss";
</style>
