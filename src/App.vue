<template>
  <div class="global">
    <div class="cadre">
      <div class="nav">
        <navigation2 />
      </div>
      <component :is="currentView" />
      <!-- <pageAccueil />
      <restoLille /> -->
      <piedpage />
    </div>
  </div>
</template>


<script>
import navigation2 from "./components/navigation2.vue";
import pageAccueil from "./pageAccueil.vue";
import restoLille from "./restoLille.vue";
// import pdfCarteRestoLille from "./pdfCarteRestoLille.vue";
import restoRouen from "./restoRouen.vue";
import restoRouenHalles from "./restoRouenHalles.vue";
import nosProduits from "./nosProduits.vue";
import reservation from "./reservation.vue";
import piedpage from "./components/piedpage.vue";

const routes = {
  "/": pageAccueil,
  "/RestaurantLille": restoLille,
  // "/pdfCarteRestoLille": pdfCarteRestoLille,
  "/RestaurantRouen": restoRouen,
  "/RestaurantRouenHalles": restoRouenHalles,
  "/nos-produits": nosProduits,
  "/reservations": reservation,
};

export default {
  name: "App",
  components: {
    navigation2,
    pageAccueil,
    restoLille,
    // pdfCarteRestoLille,
    restoRouen,
    restoRouenHalles,
    nosProduits,
    reservation,
    piedpage,
  },

  data() {
    return {
      currentPath: window.location.hash,
    };
  },
  computed: {
    currentView() {
      return routes[this.currentPath.slice(1) || "/"] || pageAccueil;
    },
  },
  mounted() {
    window.addEventListener("hashchange", () => {
      this.currentPath = window.location.hash;
    });
  },
};
</script>


<style>
* {
  margin: 0;
  padding: 0;
  /* font-family: Verdana, Geneva, Tahoma, sans-serif; */
  font-family: "Cormorant Garamond", serif;
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
  border: 1rem solid #cd2428;
  /* width: 100vw; */
  height: 100%;
  box-sizing: border-box;
  background-color: #cd2428;
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
