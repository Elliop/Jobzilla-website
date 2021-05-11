<template>
  <v-col class="my-12 py-12">
      <v-row align="center" justify="center" class="my-12 pb-12">
          <h1 align="center" justify="center">Finally a pricing that fits<br><span class="primary--text"> Your recruiting needs</span></h1>
      </v-row>
    <v-row justify="center">
      <v-col cols="auto" class="mx-4">
        <Growtgh />
      </v-col>
      <v-col cols="auto" class="mx-4">
        <Enterprise />
      </v-col>
    </v-row>
  </v-col>
</template>

<script>
import Growtgh from "~/components/PricingPage/Growtgh";
import Enterprise from "~/components/PricingPage/Enterprise";

export default {
  components: { Growtgh, Enterprise },
  data() {
    return {};
  }
};
</script>
