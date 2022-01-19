<template>
  <div>
    <v-row align="center" justify="center">
      <v-col cols="13" sm="4">
        <div class="card d-flex justify-center align-center flex-column">
          <img class="card_img" width="50px" src="../img/image27.png" alt="" />
          <div class="card_div_text">
            <h1>Frond End</h1>
          </div>
          <div class="card_people_div">
            <img
              class="card_people_div_img"
              src="../img/Ellipse22.png"
              alt=""
            />
            <h5>Muxammadamin Tolibov</h5>
          </div>
          <div class="card_davomiy">
            <p>Davomiyligi: 9 oy</p>
          </div>
          <v-btn class="Navigation_btn mb-10" @click.stop="dialog = true">
            Bog`lanish
          </v-btn>
        </div>
      </v-col>
      <v-col cols="13" sm="4">
        <div class="card d-flex justify-center align-center flex-column">
          <img class="card_img" width="50px" src="../img/image27.png" alt="" />
          <div class="card_div_text">
            <h1>Frond End</h1>
          </div>
          <div class="card_people_div">
            <img
              class="card_people_div_img"
              src="../img/Ellipse22.png"
              alt=""
            />
            <h5>Axror Jo’rayev</h5>
          </div>
          <div class="card_davomiy">
            <p>Davomiyligi: 9 oy</p>
          </div>
          <v-btn class="Navigation_btn mb-10" @click.stop="dialog = true">
            Bog`lanish
          </v-btn>
        </div>
      </v-col>
      <v-col cols="13" sm="4">
        <div class="card d-flex justify-center align-center flex-column">
          <img class="card_img" width="50px" src="../img/image27.png" alt="" />
          <div class="card_div_text">
            <h1>Frond End</h1>
          </div>
          <div class="card_people_div">
            <img
              class="card_people_div_img"
              src="../img/Ellipse22.png"
              alt=""
            />
            <h5>Muxammadamin Tolibov</h5>
          </div>
          <div class="card_davomiy">
            <p>Davomiyligi: 3 oy</p>
          </div>
          <v-btn class="Navigation_btn mb-10" @click.stop="dialog = true">
            Bog`lanish
          </v-btn>
        </div>
      </v-col>
    </v-row>
    
    <v-dialog v-model="dialog" max-width="800">
      <v-card>
        <v-card-title class="text-h5">
          Use Google's location service?
        </v-card-title>

        <v-card-text>
          Let Google help apps determine location. This means sending anonymous
          location data to Google, even when no apps are running.
        </v-card-text>

        <v-card-actions>
          <v-spacer></v-spacer>

          <v-btn color="green darken-1" text @click="dialog = false">
            Disagree
          </v-btn>

          <v-btn color="green darken-1" text @click="dialog = false">
            Agree
          </v-btn>
        </v-card-actions>
      </v-card>
    </v-dialog>

  </div>
</template>

<script>
export default {
  data: () => ({
    dialog: false,

  }),
};
</script>

<style scoped lang="scss">
.card {
  background: #111820;
  border-radius: 15px;
  &_img {
    margin-top: 15px;
    width: 90%;
  }
  &_div_text {
    width: 100%;
    display: flex;
    justify-content: start;

    & h1 {
      margin-left: 5%;
      font-style: normal;
      font-weight: bold;
      font-size: 2rem;
      letter-spacing: -0.750316px;
      color: #ffffff;
    }
  }
  &_people_div {
    margin-top: 10px;
    width: 90%;
    display: flex;
    align-items: center;
    &_img {
      width: 3rem;
    }
    & h5 {
      font-style: normal;
      font-weight: bold;
      font-size: 1.3rem;
      line-height: 34px;
      letter-spacing: 0.5px;
      color: #ffffff;
      text-align: center;
      margin-left: 10px;
    }
  }
  &_davomiy {
    margin-top: 10px;
    width: 90%;
    & p {
      font-style: normal;
      font-weight: 600;
      font-size: 1rem;
      line-height: 27px;
      letter-spacing: 0.5px;
      color: #ffffff;
    }
  }
}
</style>