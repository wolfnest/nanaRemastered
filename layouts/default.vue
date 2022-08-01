<template>
    <v-app>
        <v-main>
            <v-card rounded="0" flat img="/bg_header.jpg" elevation="1" style="z-index: 2">
                <div class="pa-5 ml-3 mr-5">
                    <v-row class="pb-0" no-gutters justify="start" align="center">
                        <h4 style="font-family: Prompt; font-weight: 400; color: white">
                            ติดตามเราได้ที่ช่องทางอื่นๆ
                        </h4>
                        <v-icon size="30" class="pl-3" color="white">fab fa-facebook</v-icon>
                        <v-icon size="30" class="pl-3" color="white">fab fa-instagram</v-icon>
                        <v-spacer></v-spacer>
                        <v-icon size="20" class="pr-2" color="white">fas fa-bell</v-icon>
                        <h4
                            class="pr-3"
                            style="font-family: Prompt; font-weight: 400; color: white"
                        >
                            แจ้งเตือน
                        </h4>
                        <v-icon size="20" class="pr-2" color="white">fas fa-heart</v-icon>
                        <h4 style="font-family: Prompt; font-weight: 400; color: white">
                            รายการโปรด
                        </h4>
                        <v-divider vertical color="white" class="mr-3 ml-3"></v-divider>
                        <h4
                            @click="$router.push('/member')"
                            style="
                                font-family: Prompt;
                                font-weight: 300;
                                color: white;
                                cursor: pointer;
                            "
                        >
                            feryafei
                        </h4>
                    </v-row>
                </div>

                <v-divider></v-divider>

                <div class="pa-5" style="z-index: 2">
                    <v-row class="pa-5" no-gutters justify="center" align="center">
                        <v-img
                            class="ml-5 mr-10"
                            max-height="100"
                            max-width="100"
                            contain
                            src="/Nana.png"
                        ></v-img>

                        <v-text-field
                            solo
                            style="max-width: 75%"
                            hide-details="true"
                            outlined
                            v-model="title"
                            label="ค้นหาชื่อสินค้า"
                            append-icon="fas fa-search"
                        ></v-text-field>

                        <v-icon color="white" size="37" class="pl-7">fas fa-shopping-cart</v-icon>
                    </v-row>
                </div>
                <v-divider></v-divider>
                <v-row class="pt-3 pb-3" no-gutters justify="center" style="z-index: 2">
                    <h4 @click="$router.push('/')" style="cursor: pointer" class="menu pl-4 pr-4">
                        Home
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Product
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        New Product
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Best Product
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Discount
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Cosmetics
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Skincare
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Haircare
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Perfume
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Vitamin&Health
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Personal Items
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Tool&Brush
                    </h4>
                    <h4 @click="openCatalog()" style="cursor: pointer" class="menu pl-4 pr-4">
                        Counterbrand
                    </h4>
                </v-row>
            </v-card>

            <div style="background: #fcfcfc">
                <Nuxt />
            </div>

            <v-card
                rounded="0"
                color="white"
                flat
                style="z-index: 2; position: relative; bottom: 0"
            >
                <div class="pa-7"></div>
            </v-card>
            <v-card
                dark
                rounded="0"
                color="#fa72a3"
                flat
                style="z-index: 2; position: relative; bottom: 0"
            >
                <div class="pa-5">
                    <v-row
                        class="pl-5"
                        no-gutters
                        justify="start"
                        style="z-index: 2"
                        align="center"
                    >
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
        </v-main>
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
