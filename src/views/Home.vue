<template>
  <div class="home">
<div class="containerr">
  <div class="cardd">
    <h1>Login</h1>
    <v-text-field
        :rules="nameRules"
        label="First name"
        required
        dark
        style="padding: 20px;"
    ></v-text-field>
        <v-text-field
        :rules="nameRules"
        label="Password"
        required
        dark
        type="password"
        style="padding: 20px;"
    ></v-text-field>
    <v-btn
        style="margin-bottom: 10px"
        outlined
        dark
    >Login</v-btn>
  </div>
</div>
  </div>
</template>

<script>

export default {
  name: 'Home',
  data: () => ({
    nameRules: [
      v => !!v || 'Введите свой никнейм!',
    ],
  })
}
</script>

<style scoped lang="scss">
.home {
  background: rgb(255,10,85);
  background: linear-gradient(67deg, rgba(255,10,85,1) 0%, rgba(253,139,34,1) 100%);
  -moz-background-size: 100%; /* Firefox 3.6+ */
  -webkit-background-size: 100%; /* Safari 3.1+ и Chrome 4.0+ */
  -o-background-size: 100%; /* Opera 9.6+ */
  background-size: 100%; /* Современные браузеры */
  width: 100%;
  height: 100%;
}
.containerr{
  padding-top: 18%;
  padding-bottom: 19%;
}
.cardd {
  padding: 20px;
  margin-right: auto;
  margin-left: auto;
  width: 400px;
  border-radius: 5px;
  background: rgba(19, 24, 27, 0.2);
  backdrop-filter: blur(10px);
}
</style>
