<template>
    <v-card class="pa-1" max-width="380" height="130" outlined color="pink" dark>
        <v-row class="pb-1" no-gutters align="center">
            <v-col class="mr-7" cols="4"><v-img height="120px" :src="img"></v-img></v-col>
            <v-col>
                <h2 style="font-size: min(1.2vw, 22px)">Product Name</h2>
                <h3 style="font-weight: 300; font-size: min(1.1vw, 16px)">dawdawd</h3>
                <h4 style="font-weight: 300; font-size: min(0.8vw, 14px)">dawdawd</h4>
            </v-col>
        </v-row>
    </v-card>
</template>

<script>
export default { props: ['img', 'word', 'price', 'price_discount'] }
</script>

<style></style>
