<template>
  <div class="home-container">
    <div class="home-hero">
      <img
        alt="image"
        src="/playground_assets/integrityor.svg"
        class="home-image"
      />
      <button type="button" class="home-button button">
        <span>
          <span class="home-text1">Meldung einreic</span>
          <span>hen</span>
        </span>
      </button>
    </div>
    <div class="home-container1"></div>
    <div>
      <DangerousHTML
        html="<script>
  document.addEventListener('DOMContentLoaded', function() {
    // get the element with the 'scroll-top' data-role
    const scrollTopBtn = document.querySelector('[data-role='scroll-top']');
  
    // when the element is clicked
    scrollTopBtn.addEventListener('click', function() {
      // smoothly scroll to the top of the page
      window.scrollTo({
        top: 0,
        behavior: 'smooth'
      });
    });
  });
  </script>
  "
      ></DangerousHTML>
    </div>
  </div>
</template>

<script>
import DangerousHTML from 'dangerous-html/dist/vue/lib.mjs'

export default {
  name: 'Home',
  components: {
    DangerousHTML,
  },
  head: {
    title: 'Togthr template',
    meta: [
      {
        property: 'og:title',
        content: 'Togthr template',
      },
    ],
  },
}
</script>

<style scoped>
.home-container {
  width: 100%;
  display: flex;
  overflow: hidden;
  min-height: 100vh;
  align-items: center;
  flex-direction: column;
  background-color: #fff;
}
.home-hero {
  width: 1200px;
  height: 65px;
  display: flex;
  overflow: hidden;
  align-items: center;
  border-color: #ffffff;
  border-style: hidden;
  border-width: 0px;
  padding-left: 24px;
  padding-right: 24px;
  justify-content: space-between;
  background-color: #ffffff;
}
.home-image {
  width: 180px;
  object-fit: cover;
}
.home-button {
  font-size: 15px;
  font-style: normal;
  margin-top: 0px;
  font-weight: 600;
  line-height: 1.25em;
  padding-top: 12px;
  padding-left: 24px;
  border-radius: 5px;
  padding-right: 24px;
  padding-bottom: 12px;
  background-color: transparent;
  background-image: linear-gradient(180deg,#ff5500,#ff5500 41%,#ff2000 58.2%, #ff2000 100%);;
}
.home-text1 {
  background-color: transparent;
}
.home-container1 {
  width: 100%;
  height: 433px;
  display: flex;
  overflow: hidden;
  align-items: center;
  border-color: #fff;
  border-style: hidden;
  border-width: 0px;
  padding-left: 24px;
  padding-right: 24px;
  background-size: cover;
  justify-content: space-between;
  background-image: url("/playground_assets/alte1-1500w.webp");
  background-repeat: no-repeat;
  background-position: top;
}
</style>
