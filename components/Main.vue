<template>
  <v-container>
    <div class="Main">
      <v-row hidden class="d-sm-flex justify-sm-space-between">
        <v-col cols="12" sm="5">
          <h1 class="Main_text_h1">Nega CAT eng yaxshisi?</h1>
        </v-col>
        <v-col cols="12" sm="5">
          <p class="Main_text_p">
            Videolavhani ko’ring va nega aynan bizda ta’lim olishingiz
            kerakligini tushunib olasiz!
          </p>
        </v-col>
      </v-row>
      <div class="video">
        <video width="100%" height="1000%" controls>
          <source src="../img/Azon.mp4" type="video/mp4" />
        </video>
      </div>
    </div>
    <div class="CATkurs d-flex justify-space-between">
      <div class="header_img_triangle">
        <img class="header_img_triangle_t" src="../img/Polygon2.png" alt="" />
        <img class="header_img_triangle_b" src="../img/Polygon3.png" alt="" />
      </div>
      <h1 class="CATkurs_h1">
        CAT da siz quyidagi kurslarda o’qishingiz mumkin
      </h1>
      <div class="d-flex justify-end flex-column">
        <img height="15px" src="../img/Icons.png" alt="" />
      </div>
    </div>
    <div class=" mt-16">
      <v-row>
        <v-col cols="12" sm="4">
          <div class="mx-auto pa-16 d-flex align-center flex-column pa-0" max-width="344">
             <div class="frond-icon mt-5">
                <img height="32px" src="../img/code.png" alt="" />
             </div>
            <v-card-title class=" card-title">Front End</v-card-title>
            <p class="card-subtitle">Web sahifalarning interfeys qismini yaratish</p>
          </div>
        </v-col>
        <v-col cols="12" sm="4">
          <div class="mx-auto pa-16 d-flex align-center flex-column pa-0" max-width="344">
             <div style=" background: rgb(247, 224, 224) !important;" class="frond-icon mt-5">
                  <img  height="32px" src="../img/layer.png" alt="" />
             </div>
            <v-card-title class=" card-title">Web dizayn</v-card-title>
            <p class="card-subtitle">Web saytlar uchun dizayn tayyorlash</p>
          </div>
        </v-col>
        <v-col cols="12" sm="4">
          <div class="mx-auto pa-16 d-flex align-center flex-column pa-0" max-width="344">
             <div style=" background: rgb(243, 242, 205) !important;" class="frond-icon mt-5">
                  <img  height="32px" src="../img/cod.png" alt="" />
             </div>
            <v-card-title class=" card-title">Back End</v-card-title>
            <p class="card-subtitle">Python dasturlash tili yordamida Web saytlar algoritmini yaratish</p>
          </div>
        </v-col>
        <v-col cols="12" sm="4">
          <div class="mx-auto pa-16 d-flex align-center flex-column pa-0" max-width="344">
             <div style=" background: #f5f4de; !important;" class="frond-icon mt-5">  
                <img  height="32px" src="../img/align-vertically.png" alt="" />
             </div>
            <v-card-title class=" card-title">Grafik dizayn</v-card-title>
            <p class="card-subtitle">Create a platform with the best and coolest quality from us.</p>
          </div>
        </v-col>
        <v-col cols="12" sm="4">
          <div class="mx-auto pa-16 d-flex align-center flex-column pa-0" max-width="344">
             <div class="frond-icon mt-5">
                  <img  height="32px" src="../img/camera.png" alt="" />
             </div>
            <v-card-title class=" card-title">Flutter</v-card-title>
            <p class="card-subtitle">We provide Photography services, and of course with the best quality</p>
          </div>
        </v-col>
        <v-col cols="12" sm="4">
          <div class="mx-auto pa-16 d-flex align-center flex-column pa-0" max-width="344">
             <div style=" background: rgb(247, 224, 224) !important;" class="frond-icon mt-5">
                 <img  height="32px" src="../img/video-play.png" alt="" />
             </div>
            <v-card-title class=" card-title">Java</v-card-title>
            <p class="card-subtitle">Create a platform with the best and coolest quality from us.</p>
          </div>
        </v-col>
      </v-row>
    </div>
    <div  class="mt-16">
      <div style=" width:100%" class=" d-flex justify-end">
        <div class="header_img_triangle">
            <img class="header_img_triangle_t"  src="../img/Ellipse57.png" alt="">
            <img class="header_img_triangle_b"  src="../img/Ellipse58.png" alt="">
        </div> 
      </div>
       <div class=" d-flex justify-start">
        <h1 class="bizdi_kurs">Bizning kurslar</h1>
      </div>
    </div>
    <div class=" slider">
      <Card/>
    </div>
    <div>
      <forms></forms>
    </div>
  </v-container>
</template>

<script>
import Card from '~/Card/Card.vue';
import Forms from './Forms.vue';

export default {
  components: { Card, Forms }, 


     data() {
        return {
         video: null,
          };
  },
};
</script>

<style scoped  lang="scss">
.Main {
  &_text_h1 {
    font-weight: 700 !important;
    font-size: 2.5rem;
    color: #141b23;
  }
  &_text_p {
    font-size: 1rem;
    color: rgba(20, 27, 35, 0.7);
    line-height: 2.2rem;
  }
}
.video {
  width: 100%;
  margin-top: 20px;
  &-player {
    width: 100%;
  }
}
.header_img_triangle {
  width: 3rem;
  height: 3rem;
  display: flex;
  justify-content: center;
  align-content: center;
  flex-direction: column;
  position: relative;
  &_t {
    position: absolute;
    top: 0;
    width: 2rem;
  }
  &_b {
    width: 2rem;
    position: absolute;
    bottom: 0;
    right: 0.7rem;
  }
}
.CATkurs {
  margin-top: 2rem;
  &_h1 {
    font-family: "Franklin Gothic Medium", "Arial Narrow", Arial, sans-serif;
    font-style: normal;
    font-weight: bold;
    font-size: 3rem;
    line-height: 3.5rem;

    text-align: center;

    color: #141b23;
  }
}
.frond-icon{
    width: 4rem;
    height: 4rem;
    background: rgba(58, 159, 134, 0.1);
    display: flex;
    justify-content: center;
    align-items: center;
    border-radius: 50%;
   
}
.card-title{
    text-align: center;
    font-family: Nunito Sans;
    font-style: normal;
    font-weight: 600;
    font-size: 1.2rem;
    line-height: 1.7rem;
    text-align: center;
    letter-spacing: -0.750316px;
    color: #141B23;
}
.card-subtitle{
    font-family: Nunito Sans;
    font-style: normal;
    font-weight: normal;
    font-size: 1rem;
    text-align: center;
    letter-spacing: -0.500211px;
    color: rgba(20, 27, 35, 0.7);
    margin: 0 !important;
}
.bizdi_kurs{
  font-family: Nunito Sans;
  font-style: normal;
  font-weight: 800;
  font-size: 2.5rem;
  color: #141B23;
}

.kndskds{
  color: #f5f4de;
}
</style>