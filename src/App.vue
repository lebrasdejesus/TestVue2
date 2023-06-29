<template>
  <div class="global">
    <div class="cadre">
      <div class="nav">
        <navigation />
      </div>
      <pageAccueil />
      <piedpage />
    </div>
  </div>
</template>


<script>
import navigation from './components/navigation.vue';
import pageAccueil from './pageAccueil.vue';
import piedpage from './components/piedpage.vue';

export default {
  name: 'App',
  components: {
    navigation,
    pageAccueil,
    piedpage,
  },
};
</script>


<style> * {
   margin: 0;
   padding: 0;
   /* font-family: Verdana, Geneva, Tahoma, sans-serif; */
 }

 /* .global{
  box-sizing: border-box;
} */
 body {
   /* background-color: rgb(164, 164, 164); */
   margin: 0;
   padding: 0;
 }

 .nav {
   /* position: sticky;
   top: 0; */
   margin-bottom: 1rem;
 }

 .cadre {
   border: 1rem solid #CD2428;
   /* width: 100vw; */
   height: 100%;
   box-sizing: border-box;
   background-color: #CD2428;
 }
</style>


<!-- 
<script setup>
import HelloWorld from './components/HelloWorld.vue'
import TheWelcome from './components/TheWelcome.vue'
</script>

<template>
  <header>
    <img alt="Vue logo" class="logo" src="./assets/logo.svg" width="125" height="125" />

    <div class="wrapper">
      <HelloWorld msg="frgthyjukilo" />
    </div>
  </header>

  <main>
    <TheWelcome />
  </main>
</template>

<style scoped>
header {
  line-height: 1.5;
}

.logo {
  display: block;
  margin: 0 auto 2rem;
}

@media (min-width: 1024px) {
  header {
    display: flex;
    place-items: center;
    padding-right: calc(var(--section-gap) / 2);
  }

  .logo {
    margin: 0 2rem 0 0;
  }

  header .wrapper {
    display: flex;
    place-items: flex-start;
    flex-wrap: wrap;
  }
}
</style> -->
