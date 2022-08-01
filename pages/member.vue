<template>
    <div>
        <div class="pa-5 pt-10 mx-auto" style="font-family: Prompt; max-width: 1700px">
            <v-row no-gutters>
                <v-col cols="3">
                    <v-card class="pa-5" rounded="0" flat elevation="0">
                        <v-row no-gutters class="pb-5 pr-5 pt-5" align="center" justify="center">
                            <v-img
                                src="/v.png"
                                contain
                                max-width="105px"
                                max-height="105px"
                            ></v-img>
                            <h2 class="pl-5" style="font-weight: 350">John Corner</h2>
                        </v-row>
                        <v-divider></v-divider>
                        <div class="pl-15">
                            <v-row no-gutters class="pt-5" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">
                                        fa-solid fa-user
                                    </v-icon>
                                </v-col>
                                <v-col>
                                    <h2 class="text">บัญชีของฉัน</h2>
                                </v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">
                                        fa-solod fa-cart-shopping
                                    </v-icon>
                                </v-col>
                                <v-col><h2 class="text">การซื้อของฉัน</h2></v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">fas fa-bell</v-icon>
                                </v-col>

                                <v-col><h2 class="text">การแจ้งเตือน</h2></v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">fa fa-heart</v-icon>
                                </v-col>
                                <v-col><h2 class="text">รายการถูกใจของฉัน</h2></v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">
                                        fa-solid fa-tags
                                    </v-icon>
                                </v-col>
                                <v-col><h2 class="text">คูปองของฉัน</h2></v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">
                                        fa-solid fa-store
                                    </v-icon>
                                </v-col>
                                <v-col><h2 class="text">การติดตามร้านค้า</h2></v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">
                                        fa-solid fa-shop
                                    </v-icon>
                                </v-col>
                                <v-col>
                                    <h2 class="text">เปิดร้านค้ากับนานา</h2>
                                </v-col>
                            </v-row>
                            <v-row no-gutters class="pt-3" justify="start" align="center">
                                <v-col cols="2">
                                    <v-icon size="30" class="pr-5" color="pink">
                                        fa-solid fa-book
                                    </v-icon>
                                </v-col>
                                <v-col>
                                    <h2 class="text">บทความจากนานา</h2>
                                </v-col>
                            </v-row>
                        </div>
                    </v-card>
                </v-col>
                <v-col class="pl-15">
                    <v-row no-gutters class="pt-10" justify="start" align="start">
                        <h3 class="text_normal">ข้อมูลบัญชีของฉัน</h3>
                    </v-row>
                    <v-row no-gutters justify="start" align="start">
                        <h4 class="text_normal" style="font-size: 14px">
                            จัดการข้อมูลการติดต่อ และ รหัสผ่าน
                        </h4>
                    </v-row>
                    <v-row no-gutters class="pt-12" justify="start" align="start">
                        <v-col cols="4">
                            <v-img src="/cosmetic.jpg" width="260px" height="250px"></v-img>
                        </v-col>
                        <v-col>
                            <v-row no-gutters justify="start" align="center">
                                <h4 style="font-size: 16px; font-weight: 350">ชื่อผู้ใช้งาน</h4>
                            </v-row>
                            <v-row no-gutters justify="start" align="center" class="pt-1">
                                <h4 style="font-size: 18px; font-weight: 350; color: #ab0036">
                                    John Corner
                                </h4>
                            </v-row>
                            <v-row class="pt-5" no-gutters justify="start" align="center">
                                <h4 style="font-size: 16px; font-weight: 350">อีเมล</h4>
                            </v-row>
                            <v-row no-gutters justify="start" align="center" class="pt-1">
                                <h4 style="font-size: 18px; font-weight: 350; color: #ab0036">
                                    unknowgenesis@gmail.com
                                </h4>
                            </v-row>
                            <v-row class="pt-5" no-gutters justify="start" align="center">
                                <h4 style="font-size: 16px; font-weight: 350">เบอร์โทรศัพท์</h4>
                            </v-row>
                            <v-row no-gutters justify="start" align="center" class="pt-1">
                                <h4 style="font-size: 18px; font-weight: 350; color: #ab0036">
                                    0123456789
                                </h4>
                            </v-row>
                        </v-col>
                    </v-row>

                    <v-divider class="mt-5"></v-divider>

                    <v-row no-gutters class="pt-5" justify="start" align="start">
                        <h3 class="text_normal">ข้อมูลส่วนตัว</h3>
                    </v-row>
                    <v-row no-gutters justify="start" align="start">
                        <h4 class="text_normal" style="font-size: 14px">จัดการข้อมูลส่วนตัว</h4>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-10">
                        <h4 style="font-size: 16px; font-weight: 350">ชื่อ</h4>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-0">
                        <v-text-field id="id"></v-text-field>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-1">
                        <h4 style="font-size: 16px; font-weight: 350">นามสกุล</h4>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-0">
                        <v-text-field id="id"></v-text-field>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-1">
                        <h4 style="font-size: 16px; font-weight: 350">เบอร์โทรศัพท์</h4>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-0">
                        <v-text-field id="id"></v-text-field>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-1">
                        <h4 style="font-size: 16px; font-weight: 350">วันเดือนปี</h4>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-3">
                        <v-icon size="30" class="pr-5" color="pink">
                            fa-solid fa-calendar-days
                        </v-icon>
                        30/11/2539
                    </v-row>

                    <v-row no-gutters justify="start" align="center" class="pt-7">
                        <h4 style="font-size: 16px; font-weight: 350">เพศ</h4>
                    </v-row>
                    <v-row no-gutters justify="start" align="center" class="pt-0">
                        <v-radio-group row v-model="gender">
                            <v-radio label="ชาย" value="male"></v-radio>
                            <v-radio label="หญิง" value="female"></v-radio>
                            <v-radio label="อื่นๆ" value="other"></v-radio>
                        </v-radio-group>
                    </v-row>
                    <v-divider class="mt-5"></v-divider>
                    <v-row no-gutters justify="start" align="center" class="pt-3">
                        <v-spacer></v-spacer>
                        <v-btn outlined color="pink" dark width="150px">ยืนยันเปลี่ยนข้อมูล</v-btn>
                    </v-row>
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
            gender: undefined,
        }
    },
}
</script>

<style scoped>
.text {
    color: #ab0036;
    font-weight: 300;
    font-size: 18px;
}
.text_normal {
    color: #ff6193;
    font-weight: 350;
    font-size: 20px;
}
</style>
