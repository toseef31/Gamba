<template>
    <v-overlay
         
          v-if="register==true"
        >
        <div class="px-0 pb-0 mx-5 over">
        <v-row class="pr-0 pl-3 mx-3 video" no-gutters>
              <v-col class="d-flex ma-0 pa-0">
                <img
                  class="ml-n2 mt-1 zindex"
                  width="80px"
                  height="20px"
                  :src="require('@/assets/logo.png')"
                />
                <v-spacer></v-spacer>
                <v-btn class="zindex" @click="close()" icon>
                  <v-icon color="858DA0" class="mr-n1">mdi-close</v-icon>
                </v-btn>
              </v-col>
            </v-row>
            <v-row no-gutters>
              <v-col class="d-flex mx-0 mt-n16 pa-0">
                <video
                  width="100%"
                  height="auto"
                  loop
                  muted
                  autoplay="autoplay"
                >
                  <source :src="'@/assets/greeting.mp4'" type="video/mp4" />
                  <source
                    :src="require('@/assets/greeting.mp4')"
                    type="video/ogg"
                  />
                  Your browser does not support the video tag.
                </video>
              </v-col>
            </v-row>
            <v-row>
              <v-col class="w-100 mx-2 pt-0 mobile">
            <v-tabs
              background-color="#1C202C"
              v-model="tab"
              class="bid-tab mb-4 mb-sm-0 tb px-3"
              hide-slider
              centered
              center-active
              mobile-breakpoint
              grow
            >
              <v-tabs-slider></v-tabs-slider>
             
                <v-tab
                  class="text-capitalize font-weight-bold in-active"
                  ripple
                  rounded
                  :href="'#tab-0'"
                >
                  Register
                </v-tab>
             

              <v-tab
                class="text-capitalize font-weight-bold login"
                ripple
                rounded
                :href="'#tab-1'"
              >
                Login
              </v-tab>
            </v-tabs>
          </v-col>
            </v-row>
            <v-tabs-items v-model="tab" class="transparent mobile">
        <v-tab-item value="tab-1" class="mb-7">
          <div class="px-7">
            <v-form>
              <v-row class="mt-2 pt-0">
                <v-col cols="12" md="12" class="pa-0">
                  <p class="mb-2 form-label">Email or Username</p>
                  <v-text-field
                    type="email"
                    outlined
                    persistent-hint
                  ></v-text-field>
                </v-col>
              </v-row>
              <v-row class="mt-0 pt-0">
                <v-col cols="12" md="12" class="pa-0 ma-0">
                  <p class="mb-2 form-label">Password</p>
                  <v-text-field
                    :append-icon="showPassword ? 'mdi-eye' : 'mdi-eye-off'"
                    :type="showPassword ? 'text' : 'password'"
                    outlined
                  ></v-text-field>

                  <p
                    class="mb-0 text-right mt-n4 forgot-password"
                    color="#4affd4"
                  >
                    Forgot password?
                  </p>
                </v-col>
              </v-row>
              <v-row>
                <v-col class="mb-0"
                  ><p class="form-label text-center mb-1">Verification code</p>
                  <v-otp-input length="6" class="otp px-4"></v-otp-input></v-col
              ></v-row>
              <v-row class="pt-1 bottom mt-3">
                <v-col class="pa-0 mt-2">
                  <v-btn
                    type="submit"
                    color="#ffff"
                    block
                    class="py-6 text-h6 text-capitalize btn"
                  >
                    Log in
                  </v-btn>
                </v-col>
              </v-row>
            </v-form>
            <v-row wrap no-gutters class="mt-9 mx-n1">
              <v-col class="text-center">
                <h2>
                  <span>OR</span>
                </h2>
              </v-col>
            </v-row>
            <v-row class="social-row">
              <v-col class="d-flex justify-space-between py-0 px-0">
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="34px"
                    :src="require('@/assets/google.png')"
                  />
                </v-btn>
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="16px"
                    :src="require('@/assets/facebook.png')"
                  />
                </v-btn>
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="34px"
                    :src="require('@/assets/vector.png')"
                  />
                </v-btn>
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="34px"
                    :src="require('@/assets/twitter.png')"
                  />
                </v-btn>
              </v-col>
            </v-row>
          </div>
        </v-tab-item>
      </v-tabs-items>
            <v-tabs-items v-model="tab" :dark="false" class="transparent mobile">
              <v-tab-item value="tab-0" class="mb-7">
                <div class="px-7">
                  <v-form
                    ref="form"
                   
                  >
                    <v-row class="mt-2 pt-0">
                      <v-col cols="12" md="12" class="pa-0">
                        <p class="mb-2 form-label">
                          Email Address
                        </p>
                        <v-text-field
                          type="email"
                         
                         
                          outlined
                          
                          persistent-hint
                          class="input-fields"
                        ></v-text-field>
                      </v-col>
                    </v-row>
                    <v-row class="mt-0 pt-0">
                      <v-col cols="12" md="12" class="pa-0">
                        <p class="mb-2 form-label">
                          Username
                        </p>
                        <v-text-field
                          
                          type="text"
                          name="name"
                          
                          outlined
                          
                          persistent-hint
                        ></v-text-field>
                      </v-col>
                    </v-row>
                    <v-row class="mt-0 pt-0">
                      <v-col cols="12" md="12" class="pa-0 ma-0">
                        <p class="mb-2 form-label">
                          Password
                        </p>
                        <v-text-field
                         
                          :append-icon="
                            showPassword ? 'mdi-eye' : 'mdi-eye-off'
                          "
                          :type="showPassword ? 'text' : 'password'"
                          name="password"
                          
                          outlined
                         
                        ></v-text-field>
                        <v-row class="pr-0 pl-0 mx-0" no-gutters>
                          <v-col class="d-flex ma-0 pa-0">
                            <p class="mb-0 form-label">
                              Referal code (optional)
                            </p>
                            <v-spacer></v-spacer>
                            <svg
                              v-if="showInput == false"
                              @click="toggle()"
                              class="svg-icon-a"
                              viewBox="0 0 24 24"
                            >
                              <path
                                fill="currentColor"
                                d="M7.41,8.58L12,13.17L16.59,8.58L18,10L12,16L6,10L7.41,8.58Z"
                              />
                            </svg>
                            <svg
                              @click="toggle()"
                              v-if="showInput == true"
                              class="svg-icon-b"
                              viewBox="0 0 24 24"
                            >
                              <path
                                fill="currentColor"
                                d="M7.41,15.41L12,10.83L16.59,15.41L18,14L12,8L6,14L7.41,15.41Z"
                              />
                            </svg>
                          </v-col>
                        </v-row>
                        <v-text-field
                          
                          hide-details
                          v-if="showInput"
                          class="mt-2"
                          persistent-hint
                          outlined
                        ></v-text-field>
                        <v-checkbox
                          class="checkbox mt-0 pt-0 mb-n2"
                          
                          :label="`I agree with your agreement, and confirm that I am at least 18 years old!`"
                        ></v-checkbox>
                      </v-col>
                    </v-row>
                  
                    <v-row class="pt-0 bottom mt-1">
                      <v-col class="pa-0 mt-0">
                        <v-btn
                          type="submit"
                          color="primary"
                          
                          block
                          class="py-6 text-h6 text-capitalize btn"
                        >
                          Register
                        </v-btn>
                      </v-col>
                    </v-row>
                  </v-form>
                  <v-row wrap no-gutters class="mt-9 mx-n1">
                    <v-col class="text-center">
                      <h2>
                        <span>OR</span>
                      </h2>
                    </v-col>
                  </v-row>
                  <v-row class="social-row">
              <v-col class="d-flex justify-space-between py-0 px-0">
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="34px"
                    :src="require('@/assets/google.png')"
                  />
                </v-btn>
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="16px"
                    :src="require('@/assets/facebook.png')"
                  />
                </v-btn>
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="34px"
                    :src="require('@/assets/vector.png')"
                  />
                </v-btn>
                <v-btn class="social" icon>
                  <img
                    class="mt-0"
                    width="34px"
                    :src="require('@/assets/twitter.png')"
                  />
                </v-btn>
              </v-col>
            </v-row>
                </div>
              </v-tab-item>
            </v-tabs-items>
        </div>
        </v-overlay>
    
    
    
  </template>
    
    
    <script>
    
  export default {
    components: {},
    name: "RegisterPop",
    data() {
      return {
        register:false,
        isActive: true,
      showInput: false,
      tab: "tab-0",
      };
    },
    created() {
    this.$root.$on("register", (data) => {
      
        this.register = data;
      console.login("register",this.register);
      
    });
   
  },
    methods: {
      close(){
        this.register = false;
      },
      toggle(){
        this.showInput=!this.showInput;
        console.log("clicked",this.showInput);
    }
    },
  };
  </script>
    <style scoped>
    ::v-deep .v-toolbar__content{
      padding-right: 0px!important;
      padding-left: 0px!important;
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
    color: #67fde2!important;;
  }
  .over {
  background-color: #212530 !important;
  border-radius: 6px;
  border: 1px solid 858da0 !important;
  width: 412px;

left: 744px;
top: 161px;
}
.zindex {
  z-index: 10;
}

.social {
  background: linear-gradient(180deg, #343A47 0%, #2C3140 100%);
border-bottom: 1px solid #3F4655;
border-radius: 12px;
  padding: 26px 37px;
}
.v-tab-bar {
  background-color: #1e1e1e !important;
  
}
.bid-tab {
  border-radius: 10px;
  margin-top: 15px !important;
  margin-bottom: 20px !important;
}
.v-text-field--outlined > .v-input__control > .v-input__slot {
  min-height: 45px !important;

}
::v-deep .v-input__slot {
  border-radius: 10px;
  min-height: 45px !important;
  background-color: #1c202c !important;
  box-shadow: inset 0px 4px 4px rgb(0 0 0 / 8%);
  margin-bottom: 0px;

}
::v-deep .v-input__slot fieldset {
  border-width: 0px;
  margin-bottom: 0px;
}
v-tab-item {
  font-size: 1rem;
  padding: 20px 63px!important;
  height: 49px;
}
::v-deep .v-label {
  font-size: 12px;
  color: rgb(133, 141, 160) !important;
}
::v-deep .checkbox .v-input__control .v-input__slot {
  border-radius: 0px !important;
  min-height: 45px !important;
  background-color: transparent !important;
  box-shadow: inset 0px 4px 4px rgb(0 0 0 / 0%) !important;
  margin-bottom: 0px;
  
}
.v-tab--active {
    background: linear-gradient(180deg, #343A47 0%, #2C3140 100%);
border: 1.71596px solid #3F4655;
border-radius: 10px;
  padding: 20px 63px!important;
  
  padding: 0px;
  border-radius: 10px;
}
.v-btn {
  border-radius: 10px;
}
.over {
  background-color: #212530 !important;
  border-radius: 6px;
  border: 1px solid 858da0 !important;
  width: 412px;

left: 744px;
top: 161px;
}

.btn {
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  border: 2px solid #67fde2;
  box-shadow: 0px 6.1792px 18.5376px rgba(54, 190, 6, 0.11);
  border-radius: 12px;
  border-radius: 12px;
  font-weight: 700;
  border-color: #67fde2 !important;
  color: white !important;
  font-size: 18px !important;
}

::v-deep .mdi-eye-off:before {
  color: rgb(133, 141, 160) !important;
  margin-top: -10px !important;
}
::v-deep .mdi-eye:before {
  color: rgb(133, 141, 160) !important;
  margin-top: -10px !important;
}
h2 {
  width: 100%;
  text-align: center;
  border-bottom: 1px solid#858DA0;
  line-height: 0.1em;
  margin: 10px 0 20px;
  color: #858da0;
  font-size: 14px;
}
.checkbox:checked:before {
  background-color: green !important;
}
h2 span {
  color: #858da0;
  background-color: #212530;
  padding: 0 20px;
}
.form-label {
  color: #858da0 !important;
  font-size: 14px;
}
.svg-icon-a {
  width: 24px;
  height: 24px;
  cursor: pointer;
  color: rgb(133, 141, 160) !important;
}

.svg-icon-b {
  cursor: pointer;
  width: 24px;
  height: 24px;
  color: rgb(133, 141, 160) !important;
}
::v-deep .otp .v-text-field__slot {
  background: linear-gradient(180deg, #343a47 0%, #2c3140 100%) !important;
  border: 1.71596px solid #3f4655 !important;
  border-radius: 10px !important;
  padding: 4px 11px;
}
.forgot-password {
  background: radial-gradient(
      79.44% 190.83% at 47.12% 105.83%,
      #4affd4 0%,
      #008976 100%
    ),
    #858da0;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
  font-size: 14px;
  margin-right:10px;
}
.check {
  width: 16px !important;
  height: 16px !important;
  min-width: 18px !important;
  background: transparent !important;
  border: 2px solid rgb(133, 141, 160) !important;
  padding: 0px 0px !important;
  border-radius: 3px;
}
.login{
  padding: 20px 73px!important;
}
.in-active{
  padding: 20px 63px!important;
}
.uncheck {
  width: 16px !important;
  height: 16px !important;
  min-width: 18px !important;
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  border: 2px solid rgba(255, 255, 255, 0.25);
  box-shadow: 0px 6.1792px 18.5376px rgb(16 150 87 / 27%);
  backdrop-filter: blur(2.3172px);
  border-radius: 3px;
  padding: 0px 0px !important;
}
.tick {
  font-size: 14px;
}
::v-deep .v-application a,
a {
  color: #858da0;
  text-decoration: none !important;
}
.router-link-active {
  color: white !important;
}
::v-deep .theme--dark.v-btn.v-btn--disabled {
  /* color: rgba(255, 255, 255, 0.3) !important; */
  color: white !important;
}
v-tab {
  font-size: 16px;
  font-weight: 600 !important;
  
  height: 49px;
  padding: 0px;
}
@media(max-width: 524px){
.over{
  margin-top:86px!important;
  width: 380px;
}
.video{
  padding-right:20px!important;
  padding-left:20px!important;
}
.mobile{
  margin-right:1px!important;
  margin-left:1px!important;
}

}
  </style>