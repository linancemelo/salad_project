<template>
  <div class="menu-container" ref="menu">
    <div class="bg"></div>
    <div class="top d-flex justify-content-between">
      <div class="logo">
        <img
          src="https://tw.digisalad.cool/images/logo-white.png"
          class="img-fluid"
          alt=""
        />
      </div>
      <div class="btn" @click.stop="closeMenu"><i class="bi bi-x-lg"></i></div>
    </div>
    <div class="menu">
      <div class="about">
        <div class="content"></div>
        <div class="title-container d-flex ps-3">
          <div class="img">
            <img class="img-fluid" src="https://ppt.cc/fTwZMx@.png" alt="" />
          </div>
          <div class="title ms-3 mt-2">
            <h6 class="title-top mb-2">EMPOWERING BRANDS</h6>
            <h4 class="title-bottom m-0">ABOUT US<span class="dot"></span></h4>
          </div>
        </div>
      </div>
      <div class="works">
        <div class="content"></div>
        <div class="title-container d-flex ps-3">
          <div class="img">
            <img class="img-fluid" src="https://ppt.cc/fTM5ax@.png" alt="" />
          </div>
          <div class="title ms-3 mt-2">
            <h6 class="title-top mb-2">CASE STUDIES</h6>
            <h4 class="title-bottom m-0">
              WORKS<span class="dot" style="background: #26c6d0"></span>
            </h4>
          </div>
        </div>
      </div>
      <div class="careers">
        <div class="content"></div>
        <div
          class="title-container ps-4 pb-4 d-flex flex-column justify-content-end"
        >
          <div class="img align-self-start">
            <img class="img-fluid" src="https://ppt.cc/feQNAx@.png" alt="" />
          </div>
          <div class="title mt-3 align-self-start">
            <h6 class="title-top mb-2">BE COOL WITH US</h6>
            <h4 class="title-bottom m-0">CAREERS<span class="dot"></span></h4>
          </div>
        </div>
      </div>
      <div class="insights">
        <div class="content"></div>
        <div
          class="title-container ps-4 pb-4 d-flex flex-column justify-content-end"
        >
          <div class="img align-self-start">
            <img class="img-fluid" src="https://ppt.cc/fAU5rx@.png" alt="" />
          </div>
          <div class="title mt-3 align-self-start">
            <h6 class="title-top mb-2">OUR STRATEGIES</h6>
            <h4 class="title-bottom m-0">INSIGHTS<span class="dot"></span></h4>
          </div>
        </div>
      </div>
      <div class="services">
        <div class="content"></div>
        <div class="title-container d-flex ps-3">
          <div class="img">
            <img class="img-fluid" src="https://ppt.cc/f013Xx@.png" alt="" />
          </div>
          <div class="title ms-3 mt-2">
            <h6 class="title-top mb-2">AREAS OF EXPERTISE</h6>
            <h4 class="title-bottom m-0">SERVICES<span class="dot"></span></h4>
          </div>
        </div>
      </div>
      <div class="contact">
        <div class="content"></div>
        <div class="title-container d-flex ps-3">
          <div class="title ms-3 mt-2">
            <h6 class="title-top mb-2 text-dark">START YOUR JOURNEY WITH US</h6>
            <h4 class="title-bottom m-0" style="color: #26c6d0">
              CONTACT<span class="dot"></span>
            </h4>
          </div>
        </div>
      </div>
    </div>
    <div class="menu-list">
      <ul class="list-group h-100">
        <li class="list-group-item">About</li>
        <li class="list-group-item">Works</li>
        <li class="list-group-item">Careers</li>
        <li class="list-group-item">Insights</li>
        <li class="list-group-item">Services</li>
        <li class="list-group-item">Contact</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    closeMenu () {
      this.$refs.menu.style.display = 'none'
      document.documentElement.style.overflowY = 'scroll'
    }
  }
}
</script>

<style scoped lang="scss" src="@/assets/scss/Menu.scss"></style>
