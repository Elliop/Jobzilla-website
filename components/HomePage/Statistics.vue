<template>
  <v-col>
    <v-row>
      <v-card width="100%" style="margin: 8vh 0 0 0;" class="px-3 py-3" elevation="0" color="secondary">
        <v-row>
          <v-col class="text-center headline">
            <span class="font-weight-bold">1,500,000+</span>
            <br />
            <span>Developer community</span>
          </v-col>
          <v-col class="text-center headline">
            <span class="font-weight-bold">67%</span>
            <br />
            <span>Cost to hire saved</span>
          </v-col>
          <v-col class="text-center">
            <span class="font-weight-bold headline">270,000+</span>
            <br />
            <span class="title">Coding challenges completed</span>
          </v-col>
          <v-col class="text-center headline">
            <span class="font-weight-bold">98%</span>
            <br />
            <span>Customers satisfied</span>
          </v-col>
        </v-row>
      </v-card>
    </v-row>
  </v-col>
</template>

<script>
export default {
  data() {
    return {
      features: [
        {
          title: "Start your campaign",
          text: "Create assessments for your candidates",
          icon: "startup"
        },
        {
          title: "Invite candidates",
          text: "Send to your candidates an email with a link to the platform",
          icon: "invitation"
        },
        {
          title: "Cherrypick from our ranking",
          text: "Identify & advance top performers",
          icon: "favorites"
        }
      ],
    };
  }
};
</script>