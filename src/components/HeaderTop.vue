<template>
  <v-card class="back px-0" height="107px" c tile>
    <v-btn
      class="social ml-n4 mt-10"
      @click="hide()"
      v-if="image == false"
      icon
    >
      <img width="28px" :src="require('@/assets/arrow-square-left.svg')" />
    </v-btn>
    <v-btn class="social mt-10" @click="show()" v-if="image == true" icon>
      <img
        class="im"
        width="28px"
        :src="require('@/assets/arrow-square-left.svg')"
      />
    </v-btn>
    <v-container height="90px" class="my-0 pa-0 top">
      <v-toolbar class="back pa-0 px-0" height="90px">
        <v-toolbar-title class="mt-5 px-0"
          ><router-link to="/"
            ><img
              width="158px"
              height="50px"
              src="@/assets/logo.png" /></router-link
        ></v-toolbar-title>

        <v-spacer></v-spacer>
        <h2 class="white--text mr-4 font" @click="login()">log in</h2>
        <v-btn class="add mr-0" @click="register()">Register</v-btn>
      </v-toolbar>
    </v-container>
  </v-card>
</template>
  
  
  <script>
export default {
  components: {},
  name: "HeaderTop",
  data() {
    return {
      available: false,
      data: true,
      image: true,
      username: "",
    };
  },
  methods: {
    show() {
      this.$root.$emit("showhide", false);
      console.log("show,false");
      this.image = false;
    },
    login() {
      this.$root.$emit("login", true);
      this.$root.$emit("tab", "tab-1");
    },
    register() {
      this.$root.$emit("login", true);
      this.$root.$emit("tab", "tab-0");
    },
    hide() {
      this.$root.$emit("showhide", false);
      console.log("show,true");
      this.image = true;
    },
  },
};
</script>
  <style scoped>
::v-deep .v-toolbar__content {
  padding-right: 0px !important;
  padding-left: 0px !important;
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
* {
  font-family: "Proxima-Nova-Font";
}

.font {
  font-weight: 700;
  font-size: 16px;
  cursor: pointer;
}
.font:hover {
  font-weight: 800;
  color: #67fde2 !important;
}
.im {
  transform: rotate(180deg);
}
.back {
  box-shadow: none !important;
  background-color: #272a33 !important;
}
.add {
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  border: 2px solid #67fde2;
  box-shadow: 0px 6.1792px 18.5376px rgb(54 190 6 / 11%);
  border-radius: 12px;
  color: #ffffff !important;
  letter-spacing: 0px;
  text-transform: none;
  height: 49px;
  margin-top: 1px;
  min-width: 116px;
}
.top {
  margin-top: -64px !important;
}
@media (max-width: 524px) {
  .back {
    padding: 0px 10px !important;
  }
}
</style>