<template>
  <v-container>
    <div  class="Navigation" flat>
      <v-row class="d-flex justify-space-between">
        <v-col class="d-flex align-center" cols="12" sm="3">
          <img height="44px" width="132px" src="../img/CAT.png" alt="" />
        </v-col>
        <v-col cols="12" sm="6">
          <div class="d-flex justify-end">
            <v-btn icon x-large color="grey lighten-1">
              <v-icon>mdi-youtube</v-icon>
            </v-btn>
            <v-btn icon x-large color="grey lighten-1">
              <v-icon>mdi-instagram</v-icon>
            </v-btn>
            <v-btn icon x-large color="grey lighten-1">
              <v-icon>mdi-instagram</v-icon>
            </v-btn>
            <v-btn icon x-large color="grey lighten-1">
              <v-icon>mdi-facebook</v-icon>
            </v-btn>
            <div class="d-flex align-center ml-1">

              <v-btn class="Navigation_btn" @click.stop="dialog = true">
                Bog`lanish
              </v-btn>

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
          </div>
        </v-col>
      </v-row>
    </div>
  </v-container>
</template>

<script>
export default {
  name: "Navigation",
 data () {
      return {
        dialog: false,
      }
    },
};
</script>

<style scoped <style lang="scss">
   
  .Navigation{
    background: #fff !important; 
    &_btn{
         background: #3A9F86 !important;
         color: #141B23 !important;
         font-size: 0.8rem !important;
         font-weight: normal !important;
        
    }
  }
</style>