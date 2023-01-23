<template>
  <div class="back">
    <v-container>
      <v-row class="bg mt-6">
        <v-col cols="12" md="1" class="pr-0"></v-col>
        <v-col cols="12" md="4" class="text-center px-3">
          <h3 class="white--text text-center mt-5 head-join">JOIN US!</h3>
          <v-btn class="add mx-auto mt-3">Register</v-btn>
          <v-row wrap no-gutters class="mt-6 mx-0">
            <v-col class="text-center">
              <h2>
                <span class="white--text">OR</span>
              </h2>
            </v-col>
          </v-row>
          <v-row class="mx-0">
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
                  class="mt-1"
                  width="34px"
                  :src="require('@/assets/twitter.png')"
                />
              </v-btn>
            </v-col>
          </v-row>
        </v-col>
        <v-col cols="12" md="7" class="text-center pa-0">
          <img
            class="mt-n6 mx-auto im mb-n3"
            width="418px"
            height="355px"
            :src="require('@/assets/Layer-4.png')"
          />
        </v-col>
      </v-row>
      <v-row class="mt-12">
        <v-col cols="12" md="6" class="pl-0">
          <div class="d-flex">
            <img
              class="mt-1"
              width="22px"
              height="22px"
              :src="require('@/assets/Group1.png')"
            />
            <h3 class="white--text ml-2 head-3">Casino</h3>
          </div>

          <img
            width="100%"
            height="auto"
            class="border"
            :src="require('@/assets/image91.png')"
          />
          <h3 class="white--text head-3">Superior Online Casino Experience</h3>
          <p class="mt-2">
            Explore our large selection of casino games and get ready to have
            some fun. Play Slots, Live Games, Blackjack, Baccarat, Roulette and
            thousands of other games all from the comfort of your home.
          </p>
          <v-btn class="casino mx-auto mt-3">Go to Casino</v-btn>
        </v-col>
        <v-col cols="12" md="6" class="pr-0">
          <div class="d-flex">
            <img
              class="mt-1"
              width="22px"
              height="22px"
              :src="require('@/assets/Vector1.png')"
            />
            <h3 class="white--text ml-2 head-3">SportsBook</h3>
          </div>

          <img
            width="100%"
            height="auto"
            class="border"
            :src="require('@/assets/Finalized.png')"
          />
          <h3 class="white--text head-3">
            Biggest Online Sports Betting Platform
          </h3>
          <p class="mt-2">
            Bet on your favorite teams, players, and events on our sports
            betting platform with a click of a button. A Safe and secure betting
            experience with all of your favorite sports in one place.
          </p>
          <v-btn class="sport-book mx-auto mt-3">Go to Sportsbook</v-btn>
        </v-col>
      </v-row>

      <div>
        <VueSlickCarousel v-bind="settings" class="mt-12">
          <v-col class="kal bg-layer white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/_1421344023328.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal bg-layera white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/Layer_x0020_1 (1).png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal bg-layerb white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/image 89.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal bg-layerc white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/image 88.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal bg-layerd white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/coin.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/_1421344023328.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/Layer_x0020_1 (1).png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/image 89.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/image 88.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
          <v-col class="kal white--text"
            ><div class="d-flex">
              <v-col cols="4" class="pa-0"
                ><img
                  class="mt-1"
                  width="50px"
                  height="50px"
                  :src="require('@/assets/coin.png')" /></v-col
              ><v-col cols="8" class="pa-0"
                ><h4>Bitcoin</h4>
                <h4>$234,2345</h4>
                <h6>24th volume 185M</h6></v-col
              >
            </div></v-col
          >
        </VueSlickCarousel>
      </div>

      <v-row class="bg-colored px-8 mt-12">
        <v-col cols="12" md="3">
          <h3 class="white--text headup">
            Do not have Crypto?<br />
            No problem.
          </h3>
        </v-col>
        <v-col cols="12" md="6">
          <img
            class="gray"
            width="100%%"
            height="100%"
            :src="require('@/assets/card.png')"
          />
        </v-col>
        <v-col cols="12" md="1" class="pa-0 ma-0"></v-col>
        <v-col cols="12" md="2">
          <v-btn class="sport-book-crypto mx-auto mt-1">Buy Crypto</v-btn>
        </v-col>
      </v-row>
      <v-row class="bg-colored px-4 mt-16 py-10 mb-10">
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
            class="text-capitalize font-weight-bold mr-4 ml-0"
            :href="'#tab-0'"
            ripple
            rounded
          >
            All Bets
          </v-tab>
          <v-tab
            class="text-capitalize font-weight-bold mr-4 ml-0"
            :href="'#tab-1'"
            ripple
            rounded
          >
            High Roller
          </v-tab>
          <v-tab
            class="text-capitalize font-weight-bold mr-4 ml-0"
            :href="'#tab-2'"
            ripple
            rounded
          >
            Lucky Bets
          </v-tab>
        </v-tabs>
        <v-tabs-items v-model="tab">
          <v-tab-item value="tab-0">
            <v-simple-table fixed-header height="auto" class="mt-5 bg-colored">
              <template v-slot:default>
                <thead>
                  <tr>
                    <th class="text-right white--text">Game</th>
                    <th class="text-right white--text">Player</th>
                    <th class="text-right white--text">Time</th>
                    <th class="text-right white--text">Bet</th>
                    <th class="text-right white--text">Multiplier</th>
                    <th class="text-right white--text">Profit</th>
                  </tr>
                </thead>
                <tbody>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckgreen">
                        mdi-checkbox-blank-circle </v-icon
                      >+0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckred">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckgreen">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckred">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckred">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckgreen">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckred">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckgreen">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-tab-item>
          <v-tab-item value="tab-1">
            <v-simple-table fixed-header height="auto" class="mt-5 bg-colored">
              <template v-slot:default>
                <thead>
                  <tr>
                    <th class="text-right white--text">Game</th>
                    <th class="text-right white--text">Player</th>
                    <th class="text-right white--text">Time</th>
                    <th class="text-right white--text">Bet</th>
                    <th class="text-right white--text">Multiplier</th>
                    <th class="text-right white--text">Profit</th>
                  </tr>
                </thead>
                <tbody>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      <v-icon small class="mdicheckred">
                        mdi-checkbox-blank-circle
                      </v-icon>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-tab-item>
          <v-tab-item value="tab-2">
            <v-simple-table fixed-header height="auto" class="mt-5 bg-colored">
              <template v-slot:default>
                <thead>
                  <tr>
                    <th class="text-right white--text">Game</th>
                    <th class="text-right white--text">Player</th>
                    <th class="text-right white--text">Time</th>
                    <th class="text-right white--text">Bet</th>
                    <th class="text-right white--text">Multiplier</th>
                    <th class="text-right white--text">Profit</th>
                  </tr>
                </thead>
                <tbody>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr class="bg-tr py-4">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                  <tr height="79px">
                    <td>Slots</td>
                    <td>
                      <img
                        class="mt-0 mr-2 mb-n3"
                        width="30px"
                        height="30px"
                        :src="require('@/assets/iconcat.png')"
                      />Alex the Beast
                    </td>
                    <td>4:39pm</td>
                    <td>
                      0.0000003<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                    <td>7.00x</td>
                    <td>
                      +0.000034<img
                        class="mt-0 ml-1 mb-n1"
                        width="16px"
                        height="16px"
                        :src="require('@/assets/bit.png')"
                      />
                    </td>
                  </tr>
                </tbody>
              </template>
            </v-simple-table>
          </v-tab-item>
        </v-tabs-items>
      </v-row>
    </v-container>
  </div>
</template>
    
    
    <script>
import VueSlickCarousel from "vue-slick-carousel";
import "vue-slick-carousel/dist/vue-slick-carousel.css";
// optional style for arrows & dots
import "vue-slick-carousel/dist/vue-slick-carousel-theme.css";
export default {
  components: { VueSlickCarousel },

  name: "HomeMain",
  data() {
    return {
      available: false,
      data: true,
      tab: "tab-0",
      settings: {
        dots: false,
        dotsClass: "slick-dots custom-dot-class",
        edgeFriction: 0.35,
        infinite: false,
        speed: 500,
        slidesToShow: 5,
        slidesToScroll: 1,
        responsive: [
          {
            // tablet
            breakpoint: 1200,
            settings: {
              slidesToShow: 4,
            },
          },
          {
            // tablet
            breakpoint: 991,
            settings: {
              slidesToShow: 2,
            },
          },
          {
            // mobile portrait
            breakpoint: 779,
            settings: {
              slidesToShow: 2,
            },
          },
          {
            // mobile portrait
            breakpoint: 479,
            settings: {
              slidesToShow: 1,
            },
          },
        ],
      },
    };
  },
  methods: {},
};
</script>
    <style scoped>
h6 {
  font-size: 14px;
  color: #7c8497 !important;
}
::v-deep .slick-prev {
  left: -21px !important;
}
::v-deep.v-carousel__controls {
  display: none !important;
  background: rgb(0 0 0 / 0%) !important;
}
.v-data-table > .v-data-table__wrapper > table > tbody > tr > td {
  text-align: center;
  color: #7c8497 !important;
}
.v-data-table--fixed-header
  > .v-data-table__wrapper
  > table
  > thead
  > tr:nth-child(2)
  > th {
  text-transform: uppercase;
  padding: 0 77px !important;
}
::v-deep .slick-prev:before,
::v-deep .slick-next:before {
  font-family: "slick";
  font-size: 29px !important;
}
::v-deep .slick-next {
  right: -6px !important;
}
.kal {
  background: #212530;
  border: 1.87002px solid rgba(55, 60, 71, 0.53);
  box-shadow: 0px 4px 4px rgba(0, 0, 0, 0.25);
  border-radius: 10px;
  margin: 20px 5.8px;
  height: 94px;
  width: 92% !important;
}
.theme--light.v-data-table.v-data-table--fixed-header thead th {
  background: #ffffff00;
  box-shadow: inset 0 -1px 0 rgb(0 0 0 / 12%);
  text-transform: uppercase;
  padding: 0 77px !important;
}
::v-deep.slick-list[data-v-3d1a4f76] {
  margin-right: -17px !important;
  margin-left: -17px !important;
}
.gray {
  filter: grayscale(100%);
}
.bg-colored {
  background: #212530;
  border-top: 1.87002px solid rgba(55, 60, 71, 0.53);
  border-radius: 10px;
}
.v-slide-group__content.v-tabs-bar__content,
.v-data-table--fixed-header
  > .v-data-table__wrapper
  > table
  > thead
  > tr:nth-child(2)
  > th,
.v-window-item.v-window-item--active {
  color: 7c8497 !important;
  caret-color: 7c8497 !important;
  background-color: #212530 !important;
}
.bg-tr {
  background: linear-gradient(180deg, #343a47 0%, #2c3140 100%);
  border: 2.13647px solid #3f4655;
  border-radius: 5px;
}
.theme--light.v-tabs > .v-tabs-bar .v-tab:not(.v-tab--active) {
  color: #7c8497 !important;
}
::v-deep.theme--light.v-tabs > .v-tabs-bar {
  background-color: #212530 !important;
}
.v-tab--active {
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  border: 2px solid #67fde2;
  box-shadow: 0px 6.1792px 18.5376px rgba(54, 190, 6, 0.11);
  border-radius: 12px;
  color: #ffff;
}
.sport-book {
  width: 100% !important;
  height: 60px !important;
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  text-transform: none;
  border: 2px solid #67fde2;
  box-shadow: 0px 6.1792px 18.5376px rgba(54, 190, 6, 0.11);
  border-radius: 12px;
  color: white;
  font-size: 20px;
}
@media only screen and (min-device-width: 81px) and (max-device-width: 724px) {
  .im {
    width: 226px;
    height: 192px;
    margin-top: 20px !important;
  }
  .bg {
    padding: 0px 0px !important;
  }

  ::v-deep::before,
  ::after {
    color: white !important;
  }
}

.sport-book-crypto {
  width: 100% !important;
  height: 60px !important;
  float: right;
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  text-transform: none;
  border: 2px solid #67fde2;
  box-shadow: 0px 6.1792px 18.5376px rgba(54, 190, 6, 0.11);
  border-radius: 12px;
  color: white;
}
.headup {
  font-style: normal;
  font-weight: 700;
  font-size: 20px;
}
.casino {
  width: 100% !important;
  height: 60px !important;
  background: radial-gradient(
    64.23% 101.67% at 47.73% 94.17%,
    #ffdb41 0%,
    #f0b91e 100%
  );
  text-transform: none;
  border: 2px solid #ffdb95;
  box-shadow: 0px 6.1792px 18.5376px rgba(242, 190, 35, 0.11);
  border-radius: 12px;
  color: white;
  font-size: 20px;
}
* {
  font-family: "Proxima-Nova-Font";
}
p {
  font-style: normal;
  font-weight: 600;
  font-size: 18px;
  line-height: 22px;

  /* 2 */
  font-family: "Proxima-Nova-Font";
  color: #7c8497;
}
.border {
  border-radius: 39px;
  border: 1px solid;
}
.font {
  font-weight: 700;
  font-size: 16px;
  font-family: "Proxima-Nova-Font";
}
.head-join {
  font-weight: 900;
  font-size: 32px;
  font-family: "Proxima-Nova-Font";
  line-height: 39px;
}
.back {
  box-shadow: none !important;
  background: linear-gradient(180deg, #10131a 0%, #131720 100%);
  padding: 0px 20px;
}
.head-3 {
  font-weight: 700;
  font-size: 22px;
  font-family: "Proxima-Nova-Font";
}
h2 span {
  color: #858da0 !important;
  background: #1f202b !important;
  padding: 0 20px;
}
h2 {
  width: 100%;
  text-align: center;
  border-bottom: 1px solid#3D4350;
  line-height: 0.1em;
  margin: 10px 0 20px;
  color: #858da0 !important;
  font-size: 14px;
}
a {
  cursor: pointer;
}
.add {
  width: 100% !important;
  height: 60px !important;

  color: white;
  background: radial-gradient(
    79.44% 190.83% at 47.12% 105.83%,
    #4affd4 0%,
    #008976 100%
  );
  border: 2px solid #67fde2;
  box-shadow: 0px 6.1792px 18.5376px rgba(54, 190, 6, 0.11);
  border-radius: 12px;
  font-family: "Proxima-Nova-Font";
}
.social {
  background: linear-gradient(180deg, #343a47 0%, #2c3140 100%);
  border-bottom: 1px solid #3f4655;
  border-radius: 12px;
  padding: 26px 37px;
}
.bg {
  background: url("@/assets/Rectangle.png") no-repeat center center;
  background-size: cover;
  mix-blend-mode: normal;
  border-radius: 15px;
  padding: 0px 64px;
}

.bg-layer {
  background: url("@/assets/bg-layer.png") no-repeat bottom left, #212530;
  background-size: 52px 77px;
}
.bg-layera {
  background: url("@/assets/bg-layera.png") no-repeat bottom left, #212530;
  background-size: 52px 77px;
}
.bg-layerb {
  background: url("@/assets/bg-layerc.png") no-repeat bottom left, #212530;
  background-size: 52px 77px;
}
.bg-layerc {
  background: url("@/assets/bg-layerb.png") no-repeat bottom left, #212530;
  background-size: 52px 77px;
}
.bg-layerd {
  background: url("@/assets/bg-layerd.png") no-repeat bottom left, #212530;
  background-size: 52px 77px;
}
.mdicheckgreen {
  content: "\F012F";
  color: green !important;
  font-size: 7px !important;
}
.mdicheckred {
  content: "\F012F";
  color: red !important;
  font-size: 7px !important;
}
</style>