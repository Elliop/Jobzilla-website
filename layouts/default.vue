<template>
    <v-app class="body white--text">
        <Appbar />
        <v-main>
            <v-container fluid>
                <nuxt />
            </v-container>
        </v-main>
    </v-app>
</template>

<script>
import Appbar from "~/components/Appbar";

export default {
    components: { Appbar }
};
</script>

<style>
.body {
    background: linear-gradient(
        180deg,
        rgb(19, 19, 19) 17.32%,
        #e0234e 100%
    ) !important;
}
.mont {
    font-family: "Montserrat", sans-serif !important;
}
.roboto-slab {
    font-family: "Roboto Slab", sans-serif !important;
}
.roboto-condensed {
    font-family: "Roboto Condensed", sans-serif !important;
}
.mont-alt {
    font-family: "Montserrat Alternates", sans-serif !important;
}
.uppercase {
    text-transform: uppercase;
}
.lowercase {
    text-transform: lowercase;
}
.capitalize {
    text-transform: capitalize;
}
a {
    text-decoration: none;
}
</style>
