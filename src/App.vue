<template>
  <Main-container>
    <template v-slot:header>
      <Header />
    </template>
    <main>
      <router-view/>
    </main>
    <template v-slot:footer>
      <Footer />
    </template>
  </Main-container>
</template>


<script>
import '@/assets/scss/index.scss';
import Header from '@/components/Header.vue';
import MainContainer from '@/components/MainContainer.vue';
import Footer from '@/components/Footer.vue';

export default {
  components: {Header, Footer, MainContainer}
}
</script>