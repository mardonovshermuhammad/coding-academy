<template>
  <div>
    <div class="mt-sm-16 mt-7">
      <img height="20px" src="../img/Vector 13.png" alt="" />
    </div>
    <div class="mt-7 form-box">
      <h1>Kurslarimizga yozilish uchun ma’lumotlaringizni qoldiring</h1>
      <v-form v-model="valid">
        <v-container>
          <v-row class="d-flex" justify="space-between" align="center">
            <v-col cols="12" md="5">
              <v-text-field
                v-model="firstname"
                :rules="nameRules"
                :counter="30"
                label="ism familya"
                required
                clearable
              ></v-text-field>
            </v-col>
            <v-col cols="12" md="5">
              <v-text-field
                v-model="telnomer"
                :rules="telRules"
                :counter="13"
                label="Telefon nomer"
                required
                clearable
                type="Number"
              ></v-text-field>
            </v-col>

            <v-col class="mx-auto" cols="12" md="10">
              <v-textarea
                outlined
                name="input-7-4"
                label="xabarlaringizni yopzing"
                value=""
              ></v-textarea>
            </v-col>
          </v-row>
        </v-container>
      </v-form>
    </div>
  </div>
</template>

<script>
export default {
  data: () => ({
    valid: false,
    firstname: "",
    nameRules: [
      (v) => !!v || "Ism familyangizni kiritmadingiz",
      (v) => v.length <= 30 || "hariflar soni 30 tadan oshib ketti",
    ],
    telnomer: "",
    telRules: [
      (v) => !!v || "telefon nomerdi kiritmadingiz",
      (v) => v.length <= 13 || "telefon nomer xato kiritildi",
    ],
  }),
};
</script>

<style scoped lang="scss">
.form-box {
  background: rgba(30, 30, 32, 0.05);
  & h1 {
    width: 70%;
    font-family: Archivo;
    font-style: normal;
    font-weight: bold;
    font-size: 3rem;
    line-height: 65px;
    color: #141b23;
  }
}
</style>