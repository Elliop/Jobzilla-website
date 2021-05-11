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
                    <h1 align="center" justify="center">{{ avatar.text }}</h1>
                  </v-row>
                  <v-row align="center" justify="center" class="mx-10">
                    <v-avatar size="80" class="pink darken-3 mt-6" align="center" justify="center">
                      <img :src="avatar.pic" />
                    </v-avatar>
                  </v-row>
                  <v-row align="center" justify="center">
                    <h4 class="mt-2" align="center" justify="center">{{ avatar.name }}</h4>
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
          text: "JobZilla thanks for giving cvbvcbcvvbx wesome hobby",
          pic: "/avatar-1.png"
        },
        {
          name: "estarossa",
          text: "JobZillzxvds dfg df srth gfh new awesome hobby",
          pic: "/avatar-2.png"
        },
        {
          name: "SpiderX",
          text: "I love logic, math, comdfgh fgh dfgprogramming.",
          pic: "/avatar-3.png" 
        },
        {
          name: "agourrag",
          text:
            " I don't know either JobZilla thanks fw awesome hobby",
          pic: "/avatar-4.png"
        },
        {
          name: "droven",
          text:
            "JobZilla droven  thanks droven odroven r dfgh  awesome hobby",
          pic: "/avatar-5.png"
        },
        {
          name: "Joker",
          text:
            " joker df df gfd fgdh fgx JobZilla t gfd hew awesome hobby",
          pic: "/avatar-6.png"
        }
      ]
    };
  }
};
</script>