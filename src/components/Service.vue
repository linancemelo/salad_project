<template>
  <div class="service container-fluid">
    <div class="title-container" data-aos="fade-up">
      <h4 class="title">OUR INGRADIENTS<span class="dot"></span></h4>
      <img src="../../public/Vector2.png" class="img-fluid" alt="" />
      <img src="../../public/Vector2.png" class="img-fluid" alt="" />
    </div>
    <div class="description">
      Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras
      ullamcorper bibendum bibendum. Duis tincidunt urna non pretium porta. Nam
      condimentum vitae ligula vel ornare. Phasellus at semper turpis. Nunc eu
      tellus tortor. Etiam at condimentum nisl, vitae sagittis orci. Donec id
      dignissim nunc. Donec elit ante, eleifend a dolor et, venenatis facilisis
      dolor. In feugiat orci odio, sed lacinia sem elementum quis. Aliquam
      consectetur, eros et vulputate euismod, nunc leo tempor lacus, ac rhoncus
      neque eros nec lacus. Cras lobortis molestie faucibus.
    </div>
    <div class="more">
      <button class="btn">OUR SERVICE<span class="line"></span></button>
    </div>
    <div class="service-item">
      <div class="row">
        <div
          class="col-sm-6 col-lg-4"
          v-for="(i, key) in data"
          :key="key"
          data-aos="zoom-in"
        >
          <div class="item-icon">
            <img :src="i.img" class="img-fluid" alt="" />
          </div>
          <div class="item-name">{{ i.title }}</div>
          <div class="item-description">
            Cras quis nulla commodo, aliquam lectus sed, blandit augue. Cras
            ullamcorper bibendum bibendum. Duis tincidunt urna non pretium
            porta. Nam condimentum vitae ligula vel ornare.
          </div>
          <button class="btn item-more">VIEW MORE</button>
        </div>
      </div>
    </div>
    <div class="view-more">
      <a href=""
        >VIEW MORE DIGISALAD’S INGRADIENTS
      </a>
      <span class="line"></span>
    </div>
    <div class="founder" data-aos="fade-right" data-aos-duration="1500">
      <div class="info">
        <div class="info-img">
          <img src="https://ppt.cc/fjQc3x@.png" class="img-fluid" alt="" />
        </div>
        <h5>TONY NG</h5>
        <p>Founder & Creative Director</p>
      </div>
      <div class="quote">
        <div class="top-icon">
          <img src="https://ppt.cc/f20Ygx@.png" class="img-fluid" alt="" />
          <img src="https://ppt.cc/f20Ygx@.png" class="img-fluid" alt="" />
        </div>
        <p>
          A great digital work isn’t about designing beautiful pages purely. It
          is about context - how do we deliver the
          <span>right experience to the right person at the right time</span>.
          The most important thing is that your work can engage customers at
          anytime, anywhere and let users experience an entire amazing digital
          journey.
        </p>
      </div>
    </div>
  </div>
</template>

<script>
import { ref } from 'vue'
export default {
  setup () {
    const data = ref([
      {
        title: 'UX DESGIN',
        img: 'https://ppt.cc/fTwZMx@.png'
      },
      {
        title: 'UI DESGIN',
        img: 'https://ppt.cc/fTM5ax@.png'
      },
      {
        title: 'WEBSITE DEVELOPMENT',
        img: 'https://ppt.cc/feQNAx@.png'
      },
      {
        title: 'MOBILE APP DEVELOPMENT',
        img: 'https://ppt.cc/fAU5rx@.png'
      },
      {
        title: 'ECOMMERCE',
        img: 'https://ppt.cc/f7CI2x@.png'
      },
      {
        title: 'CUSTOMER LOYALTY',
        img: 'https://ppt.cc/fFMGOx@.png'
      },
      {
        title: 'DIGITAL TRANSFORMATION',
        img: 'https://ppt.cc/f6yrUx@.png'
      },
      {
        title: 'DIGITAL MARKETING',
        img: 'https://ppt.cc/ftfVix@.png'
      },
      {
        title: 'BRANDING',
        img: 'https://ppt.cc/f013Xx@.png'
      }
    ])
    return {
      data
    }
  }
}
</script>

<style scoped lang="scss" src="@/assets/scss/Service.scss"></style>
