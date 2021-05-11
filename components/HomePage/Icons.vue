<template>
  <v-col>
    <v-row align="center" justify="space-around" style="margin: 8vh 0 0 0">
      <v-col v-for="(feature, index) in features" :key="index" cols="3">
        <v-row justify="center" class="my-3">
          <v-avatar tile size="100" class="icon">
            <img :src="require(`../../assets/icons/${feature.icon}.svg`)" :alt="feature.icon" />
          </v-avatar>
        </v-row>
        <v-row justify="center">
          <h4 class="text-center font-weight-bold my-3" style="font-family: 'Montserrat Alternates', sans-serif; font-size: 25px;">{{feature.title}}</h4>
          <p class="text-center font-weight-light my-3 subtitle-1" style="font-family: 'Montserrat Alternates', sans-serif">{{feature.text}}</p>
        </v-row>
      </v-col>
    </v-row>
    <v-row style="margin: 4vh 0 0 0">
      <v-card width="100%" height="5px" color="secondary"></v-card>
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

<style scoped>
.icon
{
  animation: float 6s ease-in-out infinite;
}
@keyframes float {
  0% {
    transform: translatey(0px);
  }
  50% {
    transform: translatey(-20px);
  }
  100% {
    transform: translatey(0px);
  }
}
</style>