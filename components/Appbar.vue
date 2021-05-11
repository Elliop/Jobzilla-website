<template>
    <v-app-bar app color="accent" flat hide-on-scroll>
        <v-spacer></v-spacer>
        <n-link to="/">
            <v-hover v-slot:default="{ hover }">
                <v-toolbar-title
                    class="roboto-slab logo white--text transition-fast-in-fast-out"
                    :style="hover ? 'font-size: 36px;' : null"
                >JobZilla</v-toolbar-title>
            </v-hover>
        </n-link>
        <v-spacer></v-spacer>
        <v-hover v-slot:default="{ hover }" v-for="(btn, index) in btns" :key="index">
            <a :href="btn.route">
                <v-btn
                    nuxt
                    :color="hover ? 'pink' : 'white'"
                    class="uppercase white--text btn roboto-condensed"
                    text
                >{{btn.text}}</v-btn>
            </a>
        </v-hover>
        <v-hover v-slot:default="{ hover }">
            <v-btn
                :color="hover ? 'white' : 'pink'"
                outlined
                tile
                class="uppercase white--text btn ml-4 roboto-condensed"
            >join now</v-btn>
        </v-hover>
        <v-spacer></v-spacer>
    </v-app-bar>
</template>

<script>
export default {
    data() {
        return {
            btns: [
                { text: "pricing", route: "/pricing" },
                { text: "contact us", route: "/contact" },
                { text: "resources", route: "/" },
                { text: "login", route: "http://localhost:3000/login" }
            ]
        };
    }
};
</script>

<style scoped>
.logo {
    font-weight: bold;
    font-size: 32px;
    letter-spacing: 0.05em;
    cursor: pointer;
    text-decoration: none;
}
.btn {
    font-weight: bold;
    letter-spacing: 0.05em;
    font-size: 18px !important;
}
</style>
