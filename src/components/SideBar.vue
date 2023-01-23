<template>
  <div class="back">
    <v-row class="px-5">
      <v-col>
        <v-tabs
          v-model="tab"
          class="bid-tab mb-4 mb-sm-0"
          hide-slider
          centered
          center-active
          mobile-breakpoint
        >
          <v-tabs-slider></v-tabs-slider>

          <v-tab
            class="text-capitalize font-weight-bold ml-0"
            :href="'#tab-0'"
            @click="tabValue('1')"
            ripple
            rounded
          >
            <img
              class="mr-1"
              width="12px"
              height="12px"
              :src="require('@/assets/Group1.png')"
            />Casino
          </v-tab>
          <v-tab
            class="text-capitalize font-weight-bold ml-0"
            :href="'#tab-1'"
            @click="tabValue('2')"
            ripple
            rounded
          >
            <img
              class="mr-1"
              width="12px"
              height="12px"
              :src="require('@/assets/Vector1.png')"
            />
            Sport
          </v-tab>
        </v-tabs>
      </v-col>
    </v-row>
    <v-tabs-items v-model="tab">
      <v-tab-item value="tab-0">
        <v-row class="pr-0 pl-0 mx-7" no-gutters>
          <v-col class="d-flex ma-0 pa-0">
            <h3 class="mb-0 form-label">All Games</h3>
            <v-spacer></v-spacer>
            <svg
              v-if="showInput == false"
              @click="toggle()"
              class="svg-icon-a mt-1"
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
              class="svg-icon-b mt-1"
              viewBox="0 0 24 24"
            >
              <path
                fill="currentColor"
                d="M7.41,15.41L12,10.83L16.59,15.41L18,14L12,8L6,14L7.41,15.41Z"
              />
            </svg>
          </v-col>
        </v-row>
        <div v-if="showInput == true">
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-8" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Vector53.png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Vector54.png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
          <v-divider></v-divider>
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-8" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Frame (3).png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Frame (2).png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-4" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Frame (3).png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Group (3).png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-4" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Vector53.png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Vector54.png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
        </div>
        <v-row class="pr-0 pl-0 mx-7 mt-4" no-gutters>
          <v-col class="d-flex ma-0 pa-0">
            <h3 class="mb-0 form-label">Sports</h3>
            <v-spacer></v-spacer>
            <svg
              v-if="showInput2 == false"
              @click="toggle2()"
              class="svg-icon-a mt-1"
              viewBox="0 0 24 24"
            >
              <path
                fill="currentColor"
                d="M7.41,8.58L12,13.17L16.59,8.58L18,10L12,16L6,10L7.41,8.58Z"
              />
            </svg>
            <svg
              @click="toggle2()"
              v-if="showInput2 == true"
              class="svg-icon-b mt-1"
              viewBox="0 0 24 24"
            >
              <path
                fill="currentColor"
                d="M7.41,15.41L12,10.83L16.59,15.41L18,14L12,8L6,14L7.41,15.41Z"
              />
            </svg>
          </v-col>
        </v-row>
        <div v-if="showInput2 == true">
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-btn class="social" icon>
                <img
                  class="mt-0 mr-3"
                  width="20px"
                  height="20px"
                  :src="require('@/assets/Group (4).png')"
                />Promotions
              </v-btn>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-btn class="social" icon>
                <img
                  class="mt-0 mr-3"
                  width="20px"
                  height="20px"
                  :src="require('@/assets/Group (5).png')"
                />VIP Program
              </v-btn>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <h4 class="white--text">Language & Currency</h4>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-select
                :items="items"
                filled
                label="Select Currency"
                dense
              ></v-select>
            </v-col>
          </v-row>

          <v-row class="px-5">
            <v-col>
              <v-tabs
                v-model="tabs"
                class="lol mb-4 mb-sm-0"
                hide-slider
                centered
                center-active
                mobile-breakpoint
              >
                <v-tabs-slider></v-tabs-slider>

                <v-tab
                  class="text-capitalize font-weight-bold ml-0"
                  :href="'#tab-3'"
                  @click="tabValue('1')"
                  ripple
                  rounded
                >
                  <img
                    class=""
                    width="16px"
                    height="16px"
                    :src="require('@/assets/moon.png')"
                  />
                </v-tab>
                <v-tab
                  class="text-capitalize font-weight-bold ml-0"
                  :href="'#tab-4'"
                  @click="tabValue('2')"
                  ripple
                  rounded
                >
                  <img
                    class=""
                    width="26px"
                    height="26px"
                    :src="require('@/assets/sun.svg')"
                  />
                </v-tab>
              </v-tabs>
            </v-col>
            <v-col>
              <v-tabs-items v-model="tabs">
                <v-tab-item value="tab-3">
                  <v-row class="pr-0 pl-0 mx-0" no-gutters>
                    <v-col class="ma-0 pa-0">
                      <h4 class="white--text mt-1">Dark Mode</h4>
                      <p class="mt-1">Currently</p>
                    </v-col>
                  </v-row>
                </v-tab-item>
                <v-tab-item value="tab-4">
                  <v-row class="pr-0 pl-0 mx-0" no-gutters>
                    <v-col class="ma-0 pa-0">
                      <h4 class="white--text mt-1">Light Mode</h4>
                      <p class="mt-1">Currently</p>
                    </v-col>
                  </v-row>
                </v-tab-item>
              </v-tabs-items>
            </v-col>
          </v-row>

          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-btn class="social" icon>
                <img
                  class="mt-0 mr-3"
                  width="20px"
                  height="20px"
                  :src="require('@/assets/Group 37489.png')"
                />Live Support
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </v-tab-item>
      <v-tab-item value="tab-1">
        <v-row class="pr-0 pl-0 mx-7" no-gutters>
          <v-col class="d-flex ma-0 pa-0">
            <h3 class="mb-0 form-label">All Games</h3>
            <v-spacer></v-spacer>
            <svg
              v-if="showInput == false"
              @click="toggle()"
              class="svg-icon-a mt-1"
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
              class="svg-icon-b mt-1"
              viewBox="0 0 24 24"
            >
              <path
                fill="currentColor"
                d="M7.41,15.41L12,10.83L16.59,15.41L18,14L12,8L6,14L7.41,15.41Z"
              />
            </svg>
          </v-col>
        </v-row>
        <div v-if="showInput == true">
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-8" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Vector53.png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Vector54.png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
          <v-divider></v-divider>
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-8" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Frame (1).png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Frame (2).png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-4" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Frame (3).png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Group (3).png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3 mt-4" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="17px"
                height="15px"
                :src="require('@/assets/Vector53.png')"
              />
              <p>Favorites</p>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 my-3" no-gutters>
            <v-col class="d-flex ma-0 pa-0">
              <img
                class="mr-2"
                width="19px"
                height="17px"
                :src="require('@/assets/Vector54.png')"
              />
              <p>Recents</p>
            </v-col>
          </v-row>
        </div>
        <v-row class="pr-0 pl-0 mx-7 mt-4" no-gutters>
          <v-col class="d-flex ma-0 pa-0">
            <h3 class="mb-0 form-label">Sports</h3>
            <v-spacer></v-spacer>
            <svg
              v-if="showInput2 == false"
              @click="toggle2()"
              class="svg-icon-a mt-1"
              viewBox="0 0 24 24"
            >
              <path
                fill="currentColor"
                d="M7.41,8.58L12,13.17L16.59,8.58L18,10L12,16L6,10L7.41,8.58Z"
              />
            </svg>
            <svg
              @click="toggle2()"
              v-if="showInput2 == true"
              class="svg-icon-b mt-1"
              viewBox="0 0 24 24"
            >
              <path
                fill="currentColor"
                d="M7.41,15.41L12,10.83L16.59,15.41L18,14L12,8L6,14L7.41,15.41Z"
              />
            </svg>
          </v-col>
        </v-row>
        <div v-if="showInput2 == true">
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-btn class="social" icon>
                <img
                  class="mt-0 mr-3"
                  width="20px"
                  height="20px"
                  :src="require('@/assets/Group (4).png')"
                />Promotions
              </v-btn>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-btn class="social" icon>
                <img
                  class="mt-0 mr-3"
                  width="20px"
                  height="20px"
                  :src="require('@/assets/Group (5).png')"
                />VIP Program
              </v-btn>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <h4 class="white--text">Language & Currency</h4>
            </v-col>
          </v-row>
          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-select
                :items="items"
                filled
                label="Select Currency"
                dense
              ></v-select>
            </v-col>
          </v-row>

          <v-row class="px-5">
            <v-col>
              <v-tabs
                v-model="tabs"
                class="lol mb-4 mb-sm-0"
                hide-slider
                centered
                center-active
                mobile-breakpoint
              >
                <v-tabs-slider></v-tabs-slider>

                <v-tab
                  class="text-capitalize font-weight-bold ml-0"
                  :href="'#tab-3'"
                  @click="tabValue('1')"
                  ripple
                  rounded
                >
                  <img
                    class=""
                    width="16px"
                    height="16px"
                    :src="require('@/assets/moon.png')"
                  />
                </v-tab>
                <v-tab
                  class="text-capitalize font-weight-bold ml-0"
                  :href="'#tab-4'"
                  @click="tabValue('2')"
                  ripple
                  rounded
                >
                  <img
                    class=""
                    width="26px"
                    height="26px"
                    :src="require('@/assets/sun.svg')"
                  />
                </v-tab>
              </v-tabs>
            </v-col>
            <v-col>
              <v-tabs-items v-model="tabs">
                <v-tab-item value="tab-3">
                  <v-row class="pr-0 pl-0 mx-0" no-gutters>
                    <v-col class="ma-0 pa-0">
                      <h4 class="white--text mt-1">Dark Mode</h4>
                      <p class="mt-1">Currently</p>
                    </v-col>
                  </v-row>
                </v-tab-item>
                <v-tab-item value="tab-4">
                  <v-row class="pr-0 pl-0 mx-0" no-gutters>
                    <v-col class="ma-0 pa-0">
                      <h4 class="white--text mt-1">Light Mode</h4>
                      <p class="mt-1">Currently</p>
                    </v-col>
                  </v-row>
                </v-tab-item>
              </v-tabs-items>
            </v-col>
          </v-row>

          <v-row class="pr-0 pl-0 mx-7 mt-4">
            <v-col class="px-0">
              <v-btn class="social" icon>
                <img
                  class="mt-0 mr-3"
                  width="20px"
                  height="20px"
                  :src="require('@/assets/Group 37489.png')"
                />Live Support
              </v-btn>
            </v-col>
          </v-row>
        </div>
      </v-tab-item>
    </v-tabs-items>
  </div>
</template>
    
    
    <script>
export default {
  components: {},
  name: "SideBar",
  data() {
    return {
      available: false,
      data: true,
      showInput: false,
      showInput2: false,
      tab: "tab-0",
      tabs: "tab-3",
      items: ["English USDT", "French USDT", "Urdu USDT", "Spanish USDT"],
    };
  },
  methods: {
    toggle() {
      this.showInput = !this.showInput;
    },
    toggle2() {
      this.showInput2 = !this.showInput2;
    },
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
* {
  font-family: "Proxima-Nova-Font";
}
::v-deep .mdi-menu-down::before {
  color: white !important;
}
.lol .v-tab--active {
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  border: 1.60653px solid rgba(255, 255, 255, 0.25);
  box-shadow: 0px 6.1792px 18.5376px rgba(16, 150, 87, 0.27);
  backdrop-filter: blur(2.3172px);
  /* Note: backdrop-filter has minimal browser support */

  border-radius: 7px;
  min-width: 58px !important;
  padding: 0px !important;
}
::v-deep.v-select.v-input--dense .v-select__selection--comma ,#input-62{
  margin: -16px 4px 3px 5px!important;
    color: #7c8497 !important;
    font-size: 14px!important;
    font-weight: 600!important;
}
::v-deep .v-text-field.v-input--is-focused > .v-input__control > .v-input__slot:after{
  display:none!important;
}
::v-deep .v-select.v-text-field--enclosed:not(.v-text-field--single-line):not(.v-text-field--outlined) .v-select__selections {
    padding-top: 20px;
    cursor: pointer!important;
}
.lol .v-tab {
  min-width: 58px !important;
}
.font {
  font-weight: 700;
  font-size: 16px;
}
.v-tabs--vertical {
  align-items: end;
  flex-direction: column;
}
::v-deep.v-select__selection.v-select__selection--comma {
  color: #7c8497 !important;
}
::v-deep.mdi:before,
.mdi-set {
  color: white !important;
}
.theme--light.v-divider {
  border-color: #272a33;
  max-width: 90%;
  text-align: center;
}
.data {
  display: none;
}
.available {
  transition: visibility 0s, opacity 0.15s linear;
  display: block;
}
.back {
  background: #171b23;
  box-shadow: 0px 0px 19px rgba(0, 0, 0, 0.2);
  backdrop-filter: blur(25px);
  height: 100%;
}

.top {
  margin-top: -64px !important;
}

.social {
  width: 100%;
  height: 46px;
  font-size: 16px;
  background: #272a33;
  box-shadow: inset 0px 4px 4px rgba(0, 0, 0, 0.08);
  border-radius: 12px;
  color: white !important;
  text-transform: none;
  justify-content: left;
  padding-left: 13px !important;
}
.v-tab-bar {
  background-color: #1e1e1e !important;
}
.bid-tab {
  border-radius: 10px;
  padding-top: 35px !important;
  padding-bottom: 20px !important;
}
.v-text-field--outlined > .v-input__control > .v-input__slot {
  min-height: 45px !important;
}
.mdi-menu-down::before {
  content: "\F035D";
  color: white !important;
}
::v-deep .v-input__slot {
  border-radius: 10px;
  min-height: 45px !important;
  background: #272a33 !important;
  box-shadow: inset 0px 4px 4px rgb(0 0 0 / 8%);
  border-radius: 12px;
}
::v-deep .v-input__slot fieldset {
  border-width: 0px;
  margin-bottom: 0px;
}
v-tab-item {
  font-size: 1rem;
  padding: 20px 31px !important;
  height: 49px;
}
::v-deep .v-label {
  font-size: 12px;
  color: rgb(133, 141, 160) !important;
}
p {
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  display: flex;
  align-items: center;

  /* 2 */

  color: #7c8497;
}
::v-deep .checkbox .v-input__control .v-input__slot {
  border-radius: 0px !important;
  min-height: 45px !important;
  background-color: transparent !important;
  box-shadow: inset 0px 4px 4px rgb(0 0 0 / 0%) !important;
  margin-bottom: 0px;
}
.v-tab--active {
  background-image: linear-gradient(#343a47, #2c3140);
  padding: 0 26px !important;
  min-width: 0px !important;
  height: 49px;
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
  font-weight: 700;

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
h4 {
  font-style: normal;
  font-weight: 600;
  font-size: 16px;
  line-height: 19px;
  display: flex;
  align-items: center;

  color: #ffffff;
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
  color: #ffff !important;
  font-size: 18px;
  font-weight: 700;
}
.svg-icon-a {
  width: 24px;
  height: 24px;
  cursor: pointer;
  color: #ffff !important;
}

.svg-icon-b {
  cursor: pointer;
  width: 24px;
  height: 24px;
  color: #ffff !important;
}
.theme--light.v-tabs-items {
  background-color: #ffffff00;
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
  margin-right: 10px;
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
.login {
  padding: 20px 73px !important;
}
.in-active {
  padding: 20px 63px !important;
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
::v-deep .v-label--active{
  display:none!important;
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
::v-deep.theme--light.v-tabs > .v-tabs-bar {
  background-color: #272a33 !important;
  background: #272a33;
  box-shadow: inset 0px 4px 4px rgb(0 0 0 / 8%);
  border-radius: 10px;
  color: white !important;
}
.bid-tab.theme--light.v-tabs > .v-tabs-bar .v-tab:not(.v-tab--active) {
  color: #7c8497 !important;
  padding: 0 26px !important;
  min-width: 0px !important;
  min-width: 0px !important;
}
v-tab {
  font-size: 16px;
  font-weight: 600 !important;
  color: #7c8497 !important;
  height: 49px;
  padding: 0px;
}
@media (max-width: 524px) {
  .over {
    margin-top: 86px !important;
    min-height: 100vh !important;
  }
  
  .mobile {
    margin-right: 16px !important;
    margin-left: 16px !important;
  }
}
</style>