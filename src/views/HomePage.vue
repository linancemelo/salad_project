<template>
  <div class="wrap">
    <Menu ref="menu"></Menu>
    <div class="head d-flex">
      <button class="btn">START YOUR PROJECT</button>
      <div class="toggle" @click.prevent="openMenu">
        <span></span>
        <span></span>
        <span></span>
      </div>
    </div>
    <div class="intro">
      <div class="cover"></div>
      <div class="logo">
        <img
          src="https://tw.digisalad.cool/images/logo-white.png"
          class="img-fluid"
          alt=""
        />
      </div>
      <div class="sideTxt">
        <div class="line"></div>
        <p class="mb-0">DIGITAL AGENCY</p>
      </div>
      <div class="content">
        <p>
          WE CREATE<br />
          AMAZING<br />
          DIGITAL EXPERIENCES
        </p>
        <span class="line"></span>
        <span class="dot"></span>
      </div>
    </div>
    <About></About>
    <Service></Service>
    <Experience></Experience>
    <ProjectSlider></ProjectSlider>
  </div>
</template>

<script>
import About from '@/components/About.vue'
import Service from '@/components/Service.vue'
import Experience from '@/components/Experience.vue'
import ProjectSlider from '../components/ProjectSlider.vue'
import Menu from '@/components/Menu.vue'
export default {
  components: {
    About,
    Service,
    Experience,
    ProjectSlider,
    Menu
  },
  methods: {
    openMenu () {
      this.$refs.menu.$el.classList.add('appear')
      this.$refs.menu.$el.style.display = 'block'
      document.documentElement.style.overflowY = 'hidden'
    }
  }
}
</script>
<style scoped lang="scss" src="@/assets/scss/HomePage.scss"></style>
