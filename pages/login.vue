<template>
    <div>
        <v-card rounded="0" class="pa-3" color="#1E53B0">
            <v-row no-gutters align="center">
                <v-img
                    class="ml-5 mr-10"
                    max-height="50"
                    max-width="50"
                    contain
                    src="/Nana.png"
                ></v-img>
                <v-spacer></v-spacer>
                <h4 style="font-family: Prompt; font-weight: 400; color: white">
                    ต้องการความช่วยเหลือ
                </h4>
                <v-icon size="20" class="pl-3 pr-2" color="white">
                    fa-solid fa-magnifying-glass
                </v-icon>
            </v-row>
        </v-card>
        <v-card rounded="0" class="pt-1" color="yellow"></v-card>
        <v-img height="92vh" src="/BG.png"></v-img>
        <div
            style="
                position: absolute;
                right: 20vw;
                top: 22vh;
                font-family: prompt;
                height: 650px;
                width: 550px;
            "
            class="bg-image"
        ></div>
        <v-card
            width="550px"
            height="650px"
            style="position: absolute; right: 20vw; top: 22vh; font-family: prompt"
            rounded="0"
            flat
            class="pa-10"
            color="transparent"
        >
            <v-row no-gutters class="pt-1">
                <h1 style="font-weight: 400; z-index: 2; color: #e91e60">เข้าสู่ระบบ</h1>
            </v-row>
            <v-row no-gutters class="pt-3">
                <v-text-field color="pink" name="name" label="อีเมล" id="id"></v-text-field>
            </v-row>
            <v-row no-gutters class="pt-2">
                <v-text-field color="pink" name="name" label="รหัสผ่าน" id="id"></v-text-field>
            </v-row>
            <v-row no-gutters class="pt-5">
                <v-btn class="mx-auto" width="450px" height="55px" color="pink" dark>
                    เข้าสู่ระบบ
                </v-btn>
            </v-row>
            <v-row no-gutters class="pt-5">
                <v-btn class="mx-auto" width="450px" height="55px" color="black" outlined>
                    ลืมรหัสผ่าน ?
                </v-btn>
            </v-row>
            <v-row no-gutters class="pt-10" align="center">
                <v-divider class="mr-3" color="#e91e60"></v-divider>
                <h5 style="font-weight: 500; color: ##e91e60">หรือ</h5>
                <v-divider class="ml-3" color="#e91e60"></v-divider>
            </v-row>
            <v-row justify="center" no-gutters class="pt-5">
                <v-img max-height="100px" max-width="110px" src="/btn/fb.png"></v-img>
                <v-img class="ml-3" max-height="100px" max-width="110px" src="/btn/go.png"></v-img>
            </v-row>
            <v-row justify="center" no-gutters class="pt-7" align="center">
                <h5 style="font-weight: 400; z-index: 2">เพื่งเคยเข้ามาใน Nana ใช่หรือไม่</h5>
                <h5 class="ml-3" style="font-weight: 500; z-index: 2; color: #e91e60">
                    สมัครสมาชิก
                </h5>
            </v-row>
        </v-card>
    </div>
</template>

<script>
export default {
    layout: 'emtly',
    methods:{
        login(){
            this.$rounter.push()
        }
    }
}
</script>

<style scoped>
.bg-image {
    /* The image used */

    filter: blur(1.5rem);
    /* Add the blur effect */
    backdrop-filter: blur(50px);
}
</style>
