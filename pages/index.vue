<template>
  <v-row align="center" justify="center" class="header-container">
    <v-col>
      <Header />
      <Icons />
      <Screen />
      <Statistics />
      <Reviews />
      <Cta />
      <Footer />
    </v-col>
  </v-row>
</template>

<script>
import Header from "@/components/HomePage/Header";
import Icons from "@/components/HomePage/Icons";
import Screen from "@/components/HomePage/Screen";
import Statistics from "@/components/HomePage/Statistics";
import Reviews from "@/components/HomePage/Reviews";
import Cta from "@/components/HomePage/Cta";
import Footer from "@/components/HomePage/Footer";
export default {
  components: { Header, Icons, Screen, Statistics, Reviews, Cta, Footer }
};
</script>