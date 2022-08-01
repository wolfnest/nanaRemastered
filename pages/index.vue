<template>
    <div>
        <v-carousel
            eager
            delimiter-icon="mdi-circle"
            light
            :cycle="true"
            hide-delimiter-background
            :show-arrows="false"
            height="800px"
        >
            <v-carousel-item
                style="cursor: pointer"
                eager
                v-for="(b, i) in banner"
                :key="b.img"
                :ripple="false"
                :src="b"
            ></v-carousel-item>
        </v-carousel>
        <div class="pr-10 pl-10 pt-5 pb-5 mx-auto" style="font-family: Prompt; max-width: 1700px">
            <v-row no-gutters>
                <h1 style="font-weight: 350">หมวดหมู่สินค้า</h1>
            </v-row>
            <div class="pt-3 pb-5">
                <v-row no-gutters justify="start">
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/new.png"
                        word="สินค้ามาใหม่"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/bestsell.png"
                        word="สินค้าขายดี"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/discount.png"
                        word="สินค้าลดราคา"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/cosmatic.png"
                        word="สินค้าสำอาง"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/facecare.png"
                        word="ผลิตภัณท์ดูแลผิวหน้า"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/haircare.png"
                        word="ผลิตภัณท์ดูแลผิวกายและเส้นผม"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/gif.png"
                        word="น้ำหอม"
                    />
                    <Cardcatalog
                        style="cursor: pointer"
                        class="mr-2 mt-3"
                        img="logo/vitamin.png"
                        word="อาหารเสริมและวิตามิน"
                    />
                    <Cardcatalog class="mr-2 mt-3" img="logo/prosenal.png" word="ของใช้ส่วนตัว" />
                    <Cardcatalog class="mr-2 mt-3" img="logo/xo3.png" word="อุปกรณ์เสริมความงาม" />
                    <Cardcatalog class="mr-2 mt-3" img="logo/ic7.png" word="เคาร์เตอร์แบรนด์" />
                </v-row>
            </div>
        </div>
        <v-img height="550" src="/banner2.png"></v-img>
        <div class="pr-10 pl-10 pt-10 mx-auto" style="font-family: Prompt; max-width: 1700px">
            <v-row no-gutters>
                <h2 style="font-weight: 400; color: #ba0b54">เทรนด์สินค้าขายดี</h2>
            </v-row>
            <div class="pt-5">
                <v-row no-gutters justify="center">
                    <v-col v-for="n in 8" :key="n" cols="3" sm="5" lg="3">
                        <CardbestSeller class="mt-1" img="/cosmetic.jpg" word="สินค้ามาใหม่" />
                    </v-col>
                </v-row>
            </div>
        </div>
        <div class="pr-10 pl-10 mx-auto pt-10" style="font-family: Prompt; max-width: 1700px">
            <v-row no-gutters>
                <h2 style="font-weight: 400; color: #ba0b54">สินค้าใหม่แนะนำสำหรับคุณ</h2>
            </v-row>
            <div class="pt-1">
                <v-row no-gutters justify="start">
                    <v-col v-for="n in 8" :key="n" cols="2" sm="3" lg="2">
                        <Cardproduct class="mt-3" img="/cosmetic.jpg" word="สินค้ามาใหม่" />
                    </v-col>
                </v-row>
            </div>
        </div>
        <div class="pr-10 pl-10 mx-auto pt-10" style="font-family: Prompt; max-width: 1700px">
            <v-row no-gutters>
                <h2 style="font-weight: 400; color: #ba0b54">โปรโมชั่นออนไลน์ประจำเดือน</h2>
            </v-row>
            <div class="pt-7">
                <v-row no-gutters justify="center">
                    <v-col class="pr-1" cols="3">
                        <v-img height="700px" src="/promo/promo1.png" />
                    </v-col>
                    <v-col class="pr-1" cols="3">
                        <v-img height="700px" src="/promo/promo2.png" />
                    </v-col>
                    <v-col class="pr-1" cols="3">
                        <v-img height="700px" src="/promo/promo3.png" />
                    </v-col>
                    <v-col class="pr-1" cols="3">
                        <v-img height="700px" src="/promo/promo4.png" />
                    </v-col>
                </v-row>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    data() {
        return {
            banner: ['/banner1.png'],
        }
    },
    methods: {
        openCatalog() {
            console.log('ss')
            this.$router.push('/catalog')
        },
    },
}
</script>

<style></style>
