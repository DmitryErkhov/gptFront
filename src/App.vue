<template>
  <v-app class="d-flex flex-column h-100">
    <header class="d-flex flex-row justify-space-between align-center py-2">
      <router-link to="/" class="naming d-flex flex-row align-center">
          <img class="mr-2" src="./assets/Logo.svg" alt="(-:-)">
          <p class="gradient">notFive-GPT</p>
        </router-link>
      <nav class="d-flex flex-row align-center">
        <router-link class="mr-3" to="/chat">Chat</router-link>
        <router-link class="mr-3" to="/possibility">Возможности</router-link>
        <hr class="mr-3" style="height: 32px; border: none; border-right: 1px solid#D1C4E9;">
        <router-link class="mr-3" to="/auth">Авторизация</router-link>
        <router-link class="mr-3" to="/register">Регистрация</router-link>
        <router-link to="/profile">Профиль</router-link>
    </nav>
    </header>
    <main>
      <router-view></router-view>
    </main>
  </v-app>
</template>
<script>

export default {
    mounted() {
    },
    data: () => ({
    }),
}
</script>
<style scoped>
  main{
    width: 100%;
    flex: 1 0 auto;
  }
  .gradient{
    font-style: normal;
    font-weight: 600;
    font-size: 32px;
    background: linear-gradient(180deg, #B388FF 0%, #6200EA 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
    background-clip: text;
  }
</style>
