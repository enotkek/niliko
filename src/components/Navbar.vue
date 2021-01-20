<template>
  <div id="app">
    <v-toolbar
        color="#121212"
        class="cock"
        style="backdrop-filter: blur(40px); background: rgba(18, 18, 18, 0.2); position: fixed; z-index: 9999999"
    >
      <v-app-bar-nav-icon @click="drawer = true" class="ass"></v-app-bar-nav-icon>
      <v-toolbar-title><b class="title">Niliko</b></v-toolbar-title>
      <v-spacer></v-spacer>
      <v-toolbar-items class="fuck">
        <v-btn color="rgba(18, 18, 18, 0) " style="box-shadow: none" to="/">Login</v-btn>
        <v-btn color="rgba(18, 18, 18, 0)" style="box-shadow: none" to="/me"><v-avatar size="40px" style="padding-right: 10px"><img src="https://cdn.discordapp.com/avatars/622747295435456512/65e87a5cd21dd5f920f4f57de97f5190.webp?size=1024" alt="whut"></v-avatar> ENOTKEK3</v-btn>
      </v-toolbar-items>

      <v-navigation-drawer
          v-model="drawer"
          absolute
          temporary
          style="backdrop-filter: blur(40px); background: rgba(18, 18, 18, 0.5);"
          height="1000px"
      >
        <v-list
            nav
            dense
        >
          <v-list-item-group
              v-model="group"
              active-class="deep-purple--text text--accent-4"
          >
            <v-list-item to="/">
              <v-list-item-icon>
                <v-icon>mdi-home</v-icon>
              </v-list-item-icon>
              <v-list-item-title>ГЛАВНАЯ</v-list-item-title>
            </v-list-item>

            <v-list-item to="stats">
              <v-list-item-icon>
                <v-icon>mdi-dns</v-icon>
              </v-list-item-icon>
              <v-list-item-title>СТАТИСТИКА</v-list-item-title>
            </v-list-item>
          </v-list-item-group>
        </v-list>
      </v-navigation-drawer>
    </v-toolbar>
  </div>
</template>

<script>
export default {
  name: 'Navbar',
  data: () => ({
    drawer: false,
    group: null,
  }),
};
</script>

<style scoped lang="scss">
* {
  color: white !important;
}
.cock {
  margin-left: 25%;
  width: 50%;
}
.title {
  font-size: 30px;
}
.ass {
  display: none;
}

@media screen and (max-width: 670px) {
  .cock {
    margin-left: 0;
    width: 100%;
  }
  .fuck {
    display: none;
  }
  .ass {
    display: block;
  }
}
</style>
