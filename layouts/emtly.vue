<template>
    <v-app>
        <div>
            <Nuxt />
        </div>

        <v-card
            width="100%"
            dark
            rounded="0"
            color="#fa72a3"
            flat
            style="z-index: 2; position: absolute; bottom: 0"
        >
            <div class="pa-5">
                <v-row class="pl-5" no-gutters justify="start" style="z-index: 2" align="center">
                    <h4 style="font-weight: 300">Copyright 2020 Nana. All Right Reserved.</h4>
                    <v-spacer></v-spacer>
                    <h5 style="font-weight: 300">Follow Us On</h5>
                    <v-icon size="30" class="pl-3" color="white">fab fa-facebook</v-icon>
                    <v-icon size="30" class="pl-3" color="white">fab fa-instagram</v-icon>
                    <v-icon size="30" class="pl-3" color="white">fab fa-line</v-icon>
                    <v-img
                        class="ml-3 mb-1"
                        max-height="33"
                        max-width="33"
                        contain
                        src="/logo/shopee.png"
                    ></v-img>
                </v-row>
            </div>
        </v-card>
    </v-app>
</template>

<script>
export default {
    methods: {
        openCatalog() {
            this.$router.push('/catalog')
        },
    },
}
</script>
<style scoped>
.menu {
    font-family: Prompt;
    font-weight: 300;
    font-size: min(0.85vw, 20px);
}
.bg-image {
    /* The image used */
    background-image: url('/bg_header.png');
    /* Add the blur effect */
}
.cardColor {
    background-color: rgba(255, 255, 255, 0.5) !important;
    border-color: white !important;
}
</style>
