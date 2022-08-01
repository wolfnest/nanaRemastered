<template>
    <div>
        <div class="pa-5 pt-10 mx-auto" style="font-family: Prompt; max-width: 1700px">
            <v-row no-gutters>
                <v-col cols="3">
                    <v-card class="pa-5" rounded="0" flat elevation="1">
                        <h2 style="font-weight: 400">ช่วงราคา</h2>
                        <v-row no-gutters class="pl-5 pr-5 pt-5">
                            <v-range-slider max="50" min="-50"></v-range-slider>
                        </v-row>

                        <v-row no-gutters class="pt-0 pr-5 pl-5" justify="center">
                            <h3 style="font-weight: 300">ราคาต่ำสุด</h3>
                            <v-spacer></v-spacer>
                            <h3 style="font-weight: 300">ราคาต่ำสุด</h3>
                        </v-row>
                        <v-row no-gutters class="pt-3 pr-5 pl-5 pb-3" justify="center">
                            <v-col class="pr-5">
                                <v-text-field hide-details outlined></v-text-field>
                            </v-col>
                            <v-col>
                                <v-text-field hide-details outlined></v-text-field>
                            </v-col>
                        </v-row>
                    </v-card>
                    <v-btn class="mt-5" width="150px" color="pink" outlined>ค้นหา</v-btn>
                </v-col>
                <v-col class="pl-10">
                    <v-row no-gutters class="pt-0 pr-5 pl-5" justify="start" align="center">
                        <h3 class="pr-2" style="font-weight: 300">หมวดหมู่ :</h3>
                        <h3 style="font-weight: 400">สินค้ามาใหม่</h3>
                    </v-row>

                    <v-row no-gutters justify="start">
                        <v-col v-for="n in 8" :key="n" cols="3" sm="4" lg="3">
                            <Cardproduct class="mt-3" img="/cosmetic.jpg" word="สินค้ามาใหม่" />
                        </v-col>
                    </v-row>

                    <v-pagination class="pt-10" v-model="page" :length="4" circle></v-pagination>
                </v-col>
            </v-row>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            page: 1,
        }
    },
}
</script>

<style></style>
