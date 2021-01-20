<template>
  <div class="about">
    <div class="profile">
      <div class="profile__user">
        <v-avatar
            size="350px"
        >
          <img src="https://cdn.discordapp.com/avatars/622747295435456512/db7cdae0fcf75856718176e569e48caf.webp?size=1024" alt="Hui">
        </v-avatar>
        <br>
        <h1>EnotKEK3</h1>
        <h4>Halp</h4>
        <v-btn outlined dark style="margin-top: 30px">Подписатся</v-btn>
        <div style="margin-top: 50px">
          <h2>Статистика</h2>
          <div
          style="
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            grid-template-rows: 1fr;
            grid-column-gap: 20px;
            grid-row-gap: 20px;
          "
          >
            <div>
              <h1>32</h1>
              Подпещика
            </div>
            <div>
              <h1>666</h1>
              пастов
            </div>
            <div>
              <h1>777</h1>
              лайков
            </div>
          </div>
        </div>
      </div>
      <div class="profile__info">
        <div class="profile__banner">
          <img class="profile__bannerr" style="opacity: 0; height: 400px;" src="@/assets/wallpaper.jpg" alt="Нахуй иди">
        </div>
        <div class="profile__moreinfo">
          <div>
            <h1>Посты</h1>
            <div class="EBUCHIE_GRIDU">
              <div class="ccardd" v-for="i in 5">
                <v-avatar size="80" class="ccardd__img" >
                  <img alt="logo" src="https://cdn.discordapp.com/avatars/622747295435456512/db7cdae0fcf75856718176e569e48caf.webp?size=1024">
                </v-avatar>
                <h2>Что?</h2>
                Whut
              </div>
            </div>
          </div>
          <div>
            <h1>Биография</h1>
            Lorem ipsum dolor sit amet, consectetur adipiscing elit. Aenean tincidunt convallis justo, non suscipit risus condimentum a. Sed a dignissim erat. Cras tempus egestas magna in fringilla. Nullam tincidunt ex non dignissim ultricies. Sed interdum euismod consectetur. Cras posuere libero blandit dictum condimentum. Vestibulum varius velit quis massa molestie auctor. Curabitur gravida scelerisque quam. Vestibulum ante ipsum primis in faucibus orci luctus et ultrices posuere cubilia curae; Sed aliquam ut ex in lobortis. Sed aliquet quam arcu, eget volutpat risus congue dictum.
          </div>
        </div>
    </div>
  </div>
  </div>
</template>

<style scoped lang="scss">
.about {
  background-color: #21D4FD;
  background-image: linear-gradient(19deg, #21D4FD 0%, #B721FF 100%);

  -moz-background-size: 100%; /* Firefox 3.6+ */
  -webkit-background-size: 100%; /* Safari 3.1+ и Chrome 4.0+ */
  -o-background-size: 100%; /* Opera 9.6+ */
  background-size: 100%; /* Современные браузеры */
  width: 100%;
  padding-bottom: 100%
}
.profile {
  padding-top: 100px;
  height: inherit;
  display: grid;
  grid-template: 50px 1fr 50px / repeat(12,1fr);
  &__user {
    padding: 40px;
    grid-column: 1 / 4;
  }
  &__info {
    padding: 40px;
    grid-column: 4 / -1;
  }
  &__banner {
    width: 100%;
    height: 400px !important;
    background: url("../assets/wallpaper.jpg") no-repeat;
    background-size: 100%;
    border-radius: 25px;
    margin-bottom: 40px;
  }
  &__moreinfo {
    display: grid;
    grid-template-columns: repeat(2, 1fr);
    grid-template-rows: 1fr;
    grid-column-gap: 100px;
    grid-row-gap: 0;
  }
}
.EBUCHIE_GRIDU {
  display: grid;
  grid-template-columns: repeat(2, 1fr);
  grid-template-rows: repeat(2, 1fr);
  grid-column-gap: 20px;
  grid-row-gap: 20px;
}

.ccardd {
  margin-top: 10px;
  background: rgba(255, 255, 255, 0.2);
  width: 400px;
  border-radius: 4px;
  text-align: left;
  padding: 10px;
  backdrop-filter: blur(40px);

  &__img {
    float: right;
  }
}
</style>
