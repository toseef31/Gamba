<template>
  <v-app>
    <v-main>
      <v-row class="pa-0">
        <v-col
          cols="12"
          md="2"
          class="ma-0 pa-0 mobile"
          v-bind:class="{ available: available, data: true }"
        >
          <SideBar />
        </v-col>
        <v-col
          cols="12"
          md="10"
          class="ma-0 pa-0"
          v-bind:class="{ available: available, done: done }"
        >
        
          <HeaderTop />
          <LoginPop/>
          <HomeMain />
          <FooterBottom />
         
        </v-col>
      </v-row>
    </v-main>
  </v-app>
</template>

<script>
import HeaderTop from "./components/HeaderTop";
import HomeMain from "./components/HomeMain";
import SideBar from "./components/SideBar";
import FooterBottom from "./components/FooterBottom";
import LoginPop from "./components/LoginPop";

export default {
  name: "App",

  components: {
    LoginPop,
    HomeMain,
    HeaderTop,
    SideBar,
    FooterBottom,
  },

  data() {
    return {
      available: false,
      data: true,
      done: true,
    };
  },
  created() {
    this.$root.$on("showhide", (data) => {
      if (this.available == false) {
        this.available = this.data;
        this.done = false;
      } else if (this.available == true) {
        this.available = data;
        this.done = true;
      }
    });
   
  },
  
};
</script>
<style scoped>

@media only screen and (min-device-width: 81px) and (max-device-width: 724px) {
.mobile{
  display: none !important;;
}
}
.data {
  display: none;
}
.done {
  min-width: 100%;
}

.available {
  transition: visibility 0s, opacity 0.15s linear;
  display: block;
  transition: display 30000s;
}
@font-face {
  font-family: "Proxima-Nova-Font";
  src: local("Proxima-Nova-Font"),
    url(@/fonts/Proxima-Nova-Font.otf) format("truetype");
}
</style>