<template>
  <v-card :loading="loading" class="mx-auto my-12" max-width="500px">
    <template slot="progress">
      <v-progress-linear
        color="deep-purple"
        height="10"
        indeterminate
      ></v-progress-linear>
    </template>

    <v-img
      height="250"
      src="https://vncsi.com.vn/data/data/anhpnh/2020/05/29/1_9456.jpg"
    ></v-img>

    <v-container>
      <v-card-title>Đăng nhập</v-card-title>

      <v-card-text>
        <v-row>
          <v-btn class="blue darken-1 rounded-pill" width="100%">
            <span> Đăng nhập với </span>
            <i class="fa-brands fa-windows"></i>
          </v-btn>
        </v-row>
      </v-card-text>

      <v-divider class="mx-4"></v-divider>

      <v-card-text style="text-align: center">Hoặc đăng nhập với</v-card-text>

      <v-card-text>
        <v-chip-group
          v-model="selection"
          active-class="deep-purple accent-4 white--text"
          column
        >
          <v-chip>5:30PM</v-chip>

          <v-chip>7:30PM</v-chip>

          <v-chip>8:00PM</v-chip>

          <v-chip>9:00PM</v-chip>
        </v-chip-group>
      </v-card-text>
      <v-checkbox v-model="checkbox" label="Ghi nhớ tài khoản"></v-checkbox>
      <v-card-text>
        <v-row>
          <v-btn class="red darken-1 rounded-pill" width="100%">
            <span> Đăng nhập </span>
          </v-btn>
        </v-row>
      </v-card-text>
    </v-container>
  </v-card>
</template>

<script>
export default {
  name: "BackGround",
};
</script>

<style>
#app {
  background: url("https://wallpaper.dog/large/10868901.jpg");
}
</style>
