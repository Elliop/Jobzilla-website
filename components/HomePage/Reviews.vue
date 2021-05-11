<template>
  <v-col>
    <v-row align="center" justify="space-around" style="margin: 8vh 0 0 0">
      <h1 align="center">Why developers
        <br />
        <span class>love us</span>
      </h1>
    </v-row>
    <v-row align="center" justify="space-around" style="margin: 8vh 0 0 0">
      <v-row style="margin: 0 1vh 0 1vh">
        <v-col>
          <v-card light>
            <v-carousel cycle :show-arrows="false" :hide-delimiters="true" height="100%">
              <v-carousel-item v-for="avatar in avatars" :key="avatar.name">
                <v-col>
                  <v-row align="center" justify="center" class="my-6 mx-10">
                    <h1 class="black--text" color="primary" align="center" justify="center">{{ avatar.text }}</h1>
                  </v-row>
                  <v-row align="center" justify="center" class="mx-10">
                    <v-avatar size="80" class="pink darken-3 mt-6" align="center" justify="center">
                      <img :src="avatar.pic" />
                    </v-avatar>
                  </v-row>
                  <v-row align="center" justify="center">
                    <h3 class="mt-2 black--text" align="center" justify="center">{{ avatar.name }}</h3>
                  </v-row>
                </v-col>
              </v-carousel-item>
            </v-carousel>
          </v-card>
        </v-col>
      </v-row>
    </v-row>
  </v-col>
</template>

<script>
export default {
  data() {
    return {
      avatars: [
        {
          name: "Elliop",
          text: "JobZilla thanks for giving us this wesome hobby",
          pic: "/avatar-1.png"
        },
        {
          name: "Estarossa",
          text: "JobZilla Best way ever of learning how to solve problems",
          pic: "/avatar-2.png"
        },
        {
          name: "SpiderX",
          text: "I Found this website today! It's juste amazing!",
          pic: "/avatar-3.png" 
        },
        {
          name: "Agourrag",
          text:
            "All I can say is that JobZilla is awesome!",
          pic: "/avatar-4.png"
        },
        {
          name: "Droven",
          text:
            "JobZilla looks like a great way to learn",
          pic: "/avatar-5.png"
        },
        {
          name: "Joker",
          text:
            "JpbZilla's contest was the most fun I've had programming in a while",
          pic: "/avatar-6.png"
        }
      ]
    };
  }
};
</script>