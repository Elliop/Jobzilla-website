<template>
  <v-footer dark padless absolute>
    <v-col style="margin:  0 4vh 0 4vh">
      <v-row>
        <v-col v-for="(item, i) in items" :key="i">
          <span v-text="item.title"></span>
        </v-col>
      </v-row>

      <v-row>
        <v-col v-for="(item, i) in items" :key="i">
          <v-row>
            <v-card width="50%" height="5px" color="primary"></v-card>
          </v-row>
        </v-col>
      </v-row>

      <v-row>
        <v-col v-for="(item, i) in items" :key="i">
          <v-col v-for="(itemr, i) in item.items" :key="i" :to="item.route">
            <v-row v-text="itemr.text"></v-row>
            <v-row v-text="itemr.title"></v-row>
          </v-col>
        </v-col>
      </v-row>


      <v-row>
        <v-col>
          <span>Made with love in 1337 Khouribga © 2019 JobZilla Inc. All Rights Reserved.</span>
        </v-col>
        <v-col>
          <span>Follow us</span>
          <v-btn v-for="icon in icons" :key="icon" dark icon>
            <v-icon size="24px">{{ icon }}</v-icon>
          </v-btn>
        </v-col>
      </v-row>
    </v-col>
  </v-footer>
</template>

<script>
export default {
  data() {
    return {
      icons: ["mdi-facebook-box", "mdi-twitter", "mdi-linkedin"],
      items: [
        {
          title: "Products",
          items: [
            { text: "Source", route: "/" },
            { text: "Screen", route: "/" },
            { text: "Retain", route: "/" },
            { text: "Pricing", route: "/" }
          ]
        },
        {
          title: "Legal",
          items: [
            { text: "Terms of Service", route: "/" },
            { text: "Customer Agreement", route: "/" },
            { text: "Privacy Policy", route: "/" },
            { text: "Cookies Policy", route: "/" }
          ]
        },
        {
          title: "Resources",
          items: [
            { text: "Blog", route: "/" },
            { text: "Resources", route: "/" },
            { text: "eBooks, guides & more", route: "/" },
            { text: "Research studies", route: "/" },
            { text: "Client stories", route: "/" }
          ]
        },
        {
          title: "About",
          items: [
            { text: "About", route: "/" },
            { text: "Contact us", route: "/" }
          ]
        },
        {
          title: "Get in touch",
          items: [{ text: "+212601020304", route: "/" }]
        }
      ]
    };
  }
};
</script>