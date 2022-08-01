<template>
    <div>
        <v-text-field
            class="pt-15"
            @click="modal = true"
            v-model="date"
            prepend-icon="mdi-calendar"
            readonly
            outlined
            dense
            hide-details="true"
            v-on="on"
        ></v-text-field>

        <v-dialog v-model="modal">
            <v-date-picker v-model="date" scrollable></v-date-picker>
        </v-dialog>
    </div>
</template>

<script>
export default {
    layout: 'emtly',
    data() {
        return {
            modal: false,
            date: undefined,
        }
    },
}
</script>

<style></style>
