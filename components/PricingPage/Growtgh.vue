<template>
  <v-card class="px-5 py-5" width="500" outlined light>
    <v-col>
      <v-card-title primary-title class="justify-center font-weight-bold">
        <span>GROWTH</span>
      </v-card-title>
      <v-card-subtitle class="text-center">
        <span>For businesses looking to hire just a few developers in the next months</span>
      </v-card-subtitle>
      <v-divider class="my-5"></v-divider>
      <v-row class="mb-12 pt-3 pb-6">
        <v-spacer></v-spacer>
        <h1>
          <span>299</span>
          <sup class="font-weight-light">
            <v-icon color="primary">mdi-currency-usd</v-icon>
          </sup>
        </h1>
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
        { title: "Library of 700+ tasks" },
        { title: "Junior/Senior level questions" },
        { title: "10 custom questions" },
        { title: "Recruiter team: up to 3 users" },
        { title: "Cheating protection" },
        { title: "Phone support" },
        { title: "JonZilla Benchmark™" },
        { title: "Campaign Wizard with job roles" }
      ]
    };
  }
};
</script>