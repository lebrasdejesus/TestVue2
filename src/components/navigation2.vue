<script>
export default {
  name: "NavB",
};
</script>

<template>
  <div class="navbar">
    <div class="menulogo">
      <a href="#/"
        ><img
          class="logo"
          alt="Vue logo"
          src="../assets/navbar/Lakson-logo.png"
      /></a>
    </div>

    <div>
      <ul class="mega-menu-main">
        <li class="lvl-0">
          <a class="lvl-0-mot" href="#/">Accueil</a>
        </li>
        <li class="lvl-0">
          <a href="#/">Restaurants &nbsp; <span class="felche"></span></a>
          <ul class="mega-menu-tab">
            <li class="lvl-1">
              <ul class="lvl-2">
                <li><a href="#">Lakson - Lille</a></li>
                <li><a href="#">Lakson - Rouen</a></li>
                <li><a href="#">Lakson - Rouen - Halles Agrivin</a></li>
              </ul>
            </li>
          </ul>
        </li>
        <li class="lvl-0">
          <a href="#/">Nos produits</a>
        </li>
        <li class="lvl-0">
          <a href="#/">Réservations</a>
        </li>
      </ul>
    </div>
  </div>
</template>

<style>
.navbar {
  background-color: #cd2428;
  border: 1px solid #faf5d0;
  height: 3.5rem;
  display: grid;
  grid-template-columns: 1fr 1fr;
  /* margin: 1rem; */
  color: #faf5d0;
  font-size: 1.2rem;
  font-family: "Cormorant Garamond", serif;
  font-weight: 100;
}

.logo {
  max-height: 1.2rem;
  max-width: 80%;
  padding: 0px 0px;
}

* {
  box-sizing: border-box;
}
ul {
  margin: 0;
  padding: 0;
}
li {
  list-style: none;
}

/* .mega-menu a {
  display: block;
  color: white;
  text-decoration: none;
}
.mega-menu a:hover {
  background: rgba(80, 137, 240, 0.5);
} */

.mega-menu-main {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
  background: rgba(33, 105, 236, 0.2);
  height: 3.5rem;
}

.lvl-0 > a {
  padding: 2rem 2rem;
}
/* .lvl-0:hover > ul {
  display: flex;
} */
.lvl-0 {
  position: relative;
}
.lvl-0:hover > .mega-menu-tab {
  /*2*/
  display: flex;
}
.mega-menu-tab {
  display: none;
  position: absolute;
  top: 2.4rem;
  /* top: 1rem; */
  /* left: 0; */
  min-width: 20rem;
  background: rgba(33, 105, 236, 0.5);
  flex: 1 1 auto;
}
.lvl-1 {
  flex: 1;
  margin: 0 15px;
}

.lvl-2 {
  padding: 1rem;
}
.lvl-2 li {
  padding: 0.5rem;
  flex: 1 1 auto;
}

/* .menu {
  display: flex;
  justify-content: center;
  align-items: center;
  position: relative;
}
.bout {
  padding-right: 1.5rem;
} */
.menulogo {
  display: flex;
  justify-content: left;
  align-items: center;
  padding-left: 1rem;
}

a {
  text-decoration: none;
  color: inherit;
}
.lvl-0:hover::before {
  content: "";
  position: absolute;
  background-color: #faf5d0;
  height: 1px;
  width: 20%;
  bottom: 0.5rem;
  display: block;
}

.fleche::after {
  content: "▾";
  position: absolute;
  font-style: normal;
}
</style>