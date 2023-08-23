<script>
import Nav from './components/Nav.vue';
import Header from './components/Header.vue';
import Banner from './components/Banner.vue';
import videoEn from '@/assets/videos/EDU_Video_Final_V2_eng.mp4';
import videoDu from '@/assets/videos/Edu_Video_Deutsch_V1.mp4'

export default {
  components: {
    Nav,
    Header,
    Banner
  },
  data() {
    return {
      videoEn,
      videoDu
    }
  }
}
</script>

<template>
  <Nav />
  <Header />
  <Banner />
  <div>
  <video controls width="320">
    <source :src="videoEn" type="video/mp4">
  </video>
  </div>
  <div>
  <video controls width="320">
    <source :src="videoDu" type="video/mp4">
  </video>
  </div>
</template>

<style>
  * {
    margin: 0;
    padding: 0;
    box-sizing: border-box;
  }
</style>
