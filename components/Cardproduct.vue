<template>
    <v-card max-width="250" height="380" elevation="1">
        <v-row no-gutters justify="center" class="pl-4 pr-4 pt-3">
            <v-img :src="img" height="200px" width="200px"></v-img>
        </v-row>
        <div class="pr-5 pl-5 pt-2">
            <v-row no-gutters justify="start">
                <h3 style="font-weight: 400">{{ word }}</h3>
            </v-row>
            <v-row class="pt-1" no-gutters justify="start" align="center">
                <v-chip class="mr-3" color="red" dark>
                    <h3 style="font-weight: 400">40 B</h3>
                </v-chip>
                <v-spacer></v-spacer>
                <h3 style="font-weight: 400; color: grey">520 B</h3>
            </v-row>
            <v-row class="pt-3" no-gutters justify="start" align="center">
                <h3 class="pl-1" style="font-weight: 300; color: red">144.00</h3>
            </v-row>
            <v-row class="pt-3 pb-2 mr-1" no-gutters justify="start" align="center">
                <v-spacer></v-spacer>
                <v-icon size="25" color="blue">fas fa-shopping-cart</v-icon>
            </v-row>
        </div>
    </v-card>
</template>

<script>
export default { props: ['img', 'word', 'price', 'discount', 'discountPercentage'] }
</script>

<style></style>
