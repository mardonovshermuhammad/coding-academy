<template>
   <v-container>
       <div class="header">
           <v-row class=" d-flex justify-space-between">
               <v-col class="d-inline-block" cols="12" sm="6">
                   <h1 class="header_h1 ">O`z</h1>
                   <h1 class="header_h1" >Web-saytimgizni</h1>
                   <h1 class="header_h1">yarating</h1>
                   <p class="header_p">O'zingiz xohlagan web sahifalarni endilikda o'z qo'lingiz bilan 
                       yaratishingiz va kelajak kasbini 9 oyda egallashingiz mumkin</p>

                    <div class=" d-flex justify-start">
                        <v-btn class="Navigation_btn" @click.stop="dialog = true">
                            bizning kurslar
                        </v-btn>
                    </div>
               </v-col>
               <v-col style=" height: auto;" class="d-flex justify-space-between" cols="12" md="6">
                      <div style=" height: 100%" class="d-flex justify-space-between flex-column" cols="12" sm="12">
                         <div class="d-flex justify-start">
                         <img class="header_img "  src="../img/Vector 13.png" alt="">
                       </div>
                        <div class="header_img_triangle">
                            <img class="header_img_triangle_t"  src="../img/Polygon2.png" alt="">
                            <img class="header_img_triangle_b"  src="../img/Polygon3.png" alt="">
                        </div> 
                      </div>

                      <div class="people">
                          <div class="people_border">
                              
                          </div>
                          <img class="people_img"  src="../img/people.png" alt="">
                      </div>
                      <div style=" height: 100%" class="d-flex justify-space-between flex-column" cols="12" sm="12">
                         
                        <div class="header_img_triangle">
                            <img class="header_img_triangle_t"  src="../img/Ellipse57.png" alt="">
                            <img class="header_img_triangle_b"  src="../img/Ellipse58.png" alt="">
                        </div>
                        <div class="d-flex justify-start">
                            <img class="header_img_plas"  src="../img/Icon.png" alt="">
                        </div> 
                      </div>
              
               </v-col>
               
           </v-row>
                         <v-dialog v-model="dialog" max-width="800">
                <v-card>
                  <v-card-title class="text-h5">
                    Use Google's location service?
                  </v-card-title>

                  <v-card-text>
                    Let Google help apps determine location. This means sending
                    anonymous location data to Google, even when no apps are
                    running.
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
   </v-container>
</template>

<script>

    export default {
        name: "Header",
        data () {
      return {
        dialog: false,
      }
    },
    }
</script>

<style scoped <style lang="scss">
     .header{
         &_img{
 
             width: 3rem !important;
             &_triangle{
                 width: 3rem;
                 height: 3rem;
                 display: flex;
                 justify-content: center;
                 align-content: center;
                 flex-direction: column;
                 position: relative;
                  &_t{
                      position: absolute;
                      top: 0;
                      width: 2rem ;
                     }
                 &_b{
                     width: 2rem ;
                     position: absolute;
                     bottom: 0;
                     right: 0.7rem;
                 }
             }
             &_plas{
                 width: 1rem !important;
             }
            
         }
         &_img_b{
             width: 2rem !important;
         }
         &_h1{
             font-size: 3rem;
             color: #141B23;
         }
         &_p{
             font-weight: normal;
             font-size: 1rem;
             line-height: 39px;
             letter-spacing: -0.656526px;
             color: rgba(20, 27, 35, 0.7);
         }
     }
     .people{ 
         position: relative;
         width: 60%;
         height: 100%;
         display: flex;
         justify-content: center;
         align-items: center;
     
         &_border{
             position: absolute;
             bottom: 2rem;
             transform: rotateZ(20deg);
             border: 3px solid #333;
             background: #3A9F86;
             width: 80%;
             height: 70%;
             border-radius: 2rem;
         }
         &_img{
             z-index: 10;
             position: absolute;
             bottom: 15%;
             right: 15%;
             width: 75% !important;
         }
         
     }
     .sssss{
         background: rgb(219, 160, 160);
     }
</style>
   