<template>
    <v-card
        @click="openCatalog"
        width="200"
        elevation="0"
        flat
        outlined
        style="border: 2px solid #fff3d0"
    >
        <v-row no-gutters justify="center" class="pt-7 pb-3">
            <v-img :src="img" max-height="120px" contain></v-img>
        </v-row>

        <v-row no-gutters justify="center" class="pr-5 pl-5 pb-5">
            <h5 class="text-center" style="font-weight: 400">{{ word }}</h5>
        </v-row>
    </v-card>
</template>

<script>
export default {
    props: ['img', 'word', 'id'],
    methods: {
        openCatalog() {
            this.$router.push('/catalog')
        },
    },
}
</script>

<style></style>
