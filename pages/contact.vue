<template>
  <v-col>
    <Form />
    <v-row style="margin: 20vh 0 0 0"></v-row>
    <Footer />
  </v-col>
</template>

<script>
import Form from "~/components/ContactPage/Form";
import Footer from "~/components/HomePage/Footer";

export default {
  components: { Form, Footer },
  data() {
    return {};
  }
};
</script>