<template>
  <v-row height="100%" class="mb-12">
    <v-col>
      <v-card height="100vh" color="white">
        <v-col style="padding: 6vh 0 0 6vh">
          <v-row>
            <h2>
              <span class="primary--text display-2 font-weight-black">
                Contact us
                <br />
              </span>
              <span class="accent--text display-2 font-weight-black">How can we help?</span>
            </h2>
          </v-row>
          <v-row style="padding: 2vh 0 0 0">
            <p class="accent--text title font-weight-medium">
              Ask us questions or reach out for support. A member of
              <br />our team will answer shortly!
            </p>
          </v-row>
        </v-col>
        <v-col style="padding: 4vh 6vh 0 6vh">
          <v-form>
            <v-row>
              <v-text-field light label="Your Name" style="padding: 2vh 2vh 0 0" outlined></v-text-field>
              <v-text-field
                light
                label="Your Email *"
                style="padding: 2vh 2vh 0 0"
                outlined
                required
              ></v-text-field>
            </v-row>
            <v-row>
              <v-text-field light label="Company" style="padding: 2vh 2vh 0 0" outlined></v-text-field>
            </v-row>
            <v-row>
              <v-select
                light
                label="Company size"
                style="padding: 2vh 2vh 0 0"
                outlined
                required
                :items="items"
              ></v-select>
            </v-row>
            <v-row>
              <span
                class="accent--text"
                style="padding: 2vh 0 0 0"
              >How many developers do you plan to recruit in the next 12 months? (Enter a number)</span>
            </v-row>
            <v-row>
              <v-text-field light type="number" style="padding: 1vh 2vh 0 0" outlined></v-text-field>
            </v-row>
            <v-row>
              <span class="accent--text" style="padding: 2vh 0 0 0">Message</span>
            </v-row>
            <v-row>
              <v-textarea light rows="14" style="padding: 1vh 2vh 0 0" outlined required></v-textarea>
            </v-row>
            <v-row style="padding: 2vh 0 0 0">
              <v-btn>SEND</v-btn>
            </v-row>
          </v-form>
        </v-col>
      </v-card>
    </v-col>
    <v-col>
      <v-img src="her.jpg" height="100%" width="100%" aspect-ratio="1">
      <p class="title font-weight-medium px-5" style="padding: 62vh 0 0 0">
          The challenge we organized with JobZilla had great media<br>
          coverage and very positively contributed to our Employer Brand.<br>
          On the recruitment side, the "Game of Drones" operation was a<br>
          success since it allowed us to recruit 5 developers in only one<br>
          month, including the winner of the competition.<br><br>
          <span class="font-weight-bold">Sarah Bourdin, Recruiter officer</span></p>          
      </v-img>

    </v-col>
  </v-row>
</template>

<script>
export default {
  data: () => ({
    items: [
      "Less than 10 employees",
      "10 - 50 employees",
      "More than 50 employees"
    ]
  })
};
</script>
<style scoped>
.col,
.col-1,
.col-2,
.col-3,
.col-4,
.col-5,
.col-6,
.col-7,
.col-8,
.col-9,
.col-10,
.col-11,
.col-12,
.col-auto,
.col-lg,
.col-lg-1,
.col-lg-2,
.col-lg-3,
.col-lg-4,
.col-lg-5,
.col-lg-6,
.col-lg-7,
.col-lg-8,
.col-lg-9,
.col-lg-10,
.col-lg-11,
.col-lg-12,
.col-lg-auto,
.col-md,
.col-md-1,
.col-md-2,
.col-md-3,
.col-md-4,
.col-md-5,
.col-md-6,
.col-md-7,
.col-md-8,
.col-md-9,
.col-md-10,
.col-md-11,
.col-md-12,
.col-md-auto,
.col-sm,
.col-sm-1,
.col-sm-2,
.col-sm-3,
.col-sm-4,
.col-sm-5,
.col-sm-6,
.col-sm-7,
.col-sm-8,
.col-sm-9,
.col-sm-10,
.col-sm-11,
.col-sm-12,
.col-sm-auto,
.col-xl,
.col-xl-1,
.col-xl-2,
.col-xl-3,
.col-xl-4,
.col-xl-5,
.col-xl-6,
.col-xl-7,
.col-xl-8,
.col-xl-9,
.col-xl-10,
.col-xl-11,
.col-xl-12,
.col-xl-auto {
  padding: 0;
}
.v-application .py-12 {
  padding-top: 0px !important;
  padding-bottom: 0px !important;
}
.col, .col-1, .col-2, .col-3, .col-4, .col-5, .col-6, .col-7, .col-8, .col-9, .col-10, .col-11, .col-12, .col-auto, .col-lg, .col-lg-1, .col-lg-2, .col-lg-3, .col-lg-4, .col-lg-5, .col-lg-6, .col-lg-7, .col-lg-8, .col-lg-9, .col-lg-10, .col-lg-11, .col-lg-12, .col-lg-auto, .col-md, .col-md-1, .col-md-2, .col-md-3, .col-md-4, .col-md-5, .col-md-6, .col-md-7, .col-md-8, .col-md-9, .col-md-10, .col-md-11, .col-md-12, .col-md-auto, .col-sm, .col-sm-1, .col-sm-2, .col-sm-3, .col-sm-4, .col-sm-5, .col-sm-6, .col-sm-7, .col-sm-8, .col-sm-9, .col-sm-10, .col-sm-11, .col-sm-12, .col-sm-auto, .col-xl, .col-xl-1, .col-xl-2, .col-xl-3, .col-xl-4, .col-xl-5, .col-xl-6, .col-xl-7, .col-xl-8, .col-xl-9, .col-xl-10, .col-xl-11, .col-xl-12, .col-xl-auto {
    width: 100%;
    padding: 0px;
}
</style>
<style>
.container {
    padding: 0px;

}
</style>