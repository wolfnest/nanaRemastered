<template>
    <div>
        <v-container style="max-width: 1900px; font-family: prompt" class="pt-5">
            <v-row justify="center" align="center" no-gutters class="pt-5 pa-3 mx-auto">
                <v-checkbox label="สินค้า" v-model="value" value="value"></v-checkbox>

                <v-spacer></v-spacer>
                <v-icon></v-icon>
                <h5 style="font-weight: 400; z-index: 2; color: #e91e60">
                    ลบสินค้าที่เลือกทั้งหมด
                </h5>
            </v-row>
            <v-divider></v-divider>
            <div class="mx-auto">
                <v-row no-gutters justify="start">
                    <v-col v-for="n in 8" :key="n" cols="12">
                        <v-card flat class="pa-1 mt-2" elevation="0">
                            <v-row no-gutters align="center">
                                <v-checkbox v-model="value" value="value"></v-checkbox>
                                <v-img max-height="75" max-width="75" src="/cosmetic.jpg"></v-img>
                                <h5 class="ml-5" style="font-weight: 400; z-index: 2; color: black">
                                    สินค้า Abvdefg
                                </h5>
                                <v-spacer></v-spacer>
                                <h5 class="ml-5" style="font-weight: 600; z-index: 2; color: pink">
                                    15.00 B
                                </h5>
                                <v-btn class="ml-5" color="success" icon><v-icon>+</v-icon></v-btn>
                                <v-btn color="success" icon>
                                    <v-icon></v-icon>
                                    -
                                </v-btn>
                                <v-spacer></v-spacer>
                            </v-row>
                        </v-card>
                    </v-col>
                </v-row>
                <v-divider class="mt-10"></v-divider>
            </div>
            <div class="pr-10 pl-10 mx-auto pt-10" style="font-family: Prompt; max-width: 1700px">
                <v-row no-gutters>
                    <h2 style="font-weight: 400; color: #ba0b54">สินค้าที่อาจเกี่ยวข้อง</h2>
                </v-row>
                <div class="pt-1">
                    <v-row no-gutters justify="start">
                        <v-col v-for="n in 8" :key="n" cols="2" sm="3" lg="2">
                            <Cardproduct class="mt-3" img="/cosmetic.jpg" word="สินค้ามาใหม่" />
                        </v-col>
                    </v-row>
                </div>
            </div>
        </v-container>
    </div>
</template>

<script>
export default {
    data() {
        return {}
    },
}
</script>

<style></style>
