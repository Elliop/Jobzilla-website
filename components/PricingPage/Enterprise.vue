<template>
  <v-card class="px-5 py-5" width="500" outlined light>
    <v-col>
      <v-card-title primary-title class="justify-center font-weight-bold">
        <span>ENTERPRISE</span>
      </v-card-title>
      <v-card-subtitle class="text-center">
        <span>For high-growth businesses looking to take their screening to the next level</span>
      </v-card-subtitle>
      <v-divider class="my-5"></v-divider>
      <v-row class="mb-12 pt-3 pb-6">
        <v-spacer></v-spacer>
        <h2 align="center" justify="center">
          <span>
            Pricing varies according to
            <br />your needs
          </span>
        </h2>
        <v-spacer></v-spacer>
      </v-row>
      <v-col v-for="(item, i) in items" :key="i">
        <v-row>
          <v-icon class="mr-5">mdi-check-bold</v-icon>
          <span v-text="item.title"></span>
        </v-row>
        <v-row>
          <v-divider class="my-2"></v-divider>
        </v-row>
      </v-col>
      <v-col>
        <v-btn width="100%" color="primary" large>
          <span>CONTACT US</span>
        </v-btn>
      </v-col>
    </v-col>
  </v-card>
</template>
<script>
export default {
  data() {
    return {
      items: [
        { title: "Unlimited tests and candidates" },
        { title: "Library of 1500+ tasks" },
        { title: "Junior/Senior/Expert level questions" },
        { title: "Unlimited custom questions" },
        { title: "Recruiter team: unlimited users" },
        { title: "Cheating protection" },
        { title: "Dedicated Account Manager" },
        { title: "JonZilla Benchmark™" },
        { title: "Campaign Wizard with job roles" },
        { title: "Customized branding" }
      ]
    };
  }
};
</script>