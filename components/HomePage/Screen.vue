<template>
  <v-col>
    <v-row align="center" justify="space-around" style="margin: 8vh 0 0 0">
      <h1 align="center">One integrated suite<br />
        <span class="primary--text">For tech recruiters</span>
      </h1>
    </v-row>
    <v-row align="center" justify="space-around" style="margin: 8vh 0 0 0">
      <v-row style="margin: 0 1vh 0 1vh">
        <v-col>
          <h2>Screen</h2>
          <v-divider style="margin: 1vh 0 0 0" width="20%"></v-divider>
          <p style="margin: 2vh 0 0 0">Spot the best developer for your position with our<br /> online coding tests while saving time on technical interviews.</p>
          <v-btn style="margin: 2vh 0 0 0" width="50%">TRY NOW</v-btn>
        </v-col>
        <v-col>
          <img width="100%" :src="require(`~/assets/screen/Hire.svg`)" />
        </v-col>
      </v-row>
    </v-row>
  </v-col>
</template>

<script>
export default {};
</script>