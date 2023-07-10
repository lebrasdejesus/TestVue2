<template>
  <div>
    <div class="titre-nos-produits">
      <div class="moitie">
        <h2>LAKSØN - Maison Scandinave à Lille & Rouen</h2>
        <p>Gastronomie suédoise, norvégienne et danoise​</p>
      </div>
      <div class="moitie"></div>
    </div>

    <div class="album">
      <div class="colonne">
        <div class="photo one">
          <img
            src="./assets/page-nosProduits/1-Traiteur-Dood-min-scaled.jpg"
            alt="Traiteur-Dood-min-scaled"
          />
        </div>
        <div class="photo two">
          <img
            src="./assets/page-nosProduits/2-Eise-04-decembre-2018IMG_9542-min-scaled.jpg"
            alt="2-Eise-04-decembre-2018IMG_9542-min-scaled"
          />
        </div>
        <div class="photo three">
          <img
            src="./assets/page-nosProduits/3-Eise-04-decembre-2018IMG_9330-min-scaled.jpg"
            alt="3-Eise-04-decembre-2018IMG_9330-min-scaled"
          />
        </div>
      </div>

      <div class="colonne">
        <div class="photo four">
          <img
            src="./assets/page-nosProduits/4-Saumon-Gravlax-Dood-min-scaled.jpg"
            alt="4-Saumon-Gravlax-Dood-min-scaled"
          />
        </div>
        <div class="photo five">
          <img
            src="./assets/page-nosProduits/5-Eise-04-decembre-2018IMG_9558-min-scaled.jpg"
            alt="5-Eise-04-decembre-2018IMG_9558-min-scaled"
          />
        </div>
        <div class="photo six">
          <img
            src="./assets/page-nosProduits/6-Eise-04-decembre-2018IMG_9454-min-scaled.jpg"
            alt="6-Eise-04-decembre-2018IMG_9454-min-scaled"
          />
        </div>
      </div>

      <div class="colonne">
        <div class="photo seven">
          <img
            src="./assets/page-nosProduits/7-Hareng-Dood-min-scaled.jpg"
            alt="7-Hareng-Dood-min-scaled"
          />
        </div>
        <div class="photo height">
          <img
            src="./assets/page-nosProduits/8-Eise-04-decembre-2018IMG_9508-min-scaled.jpg"
            alt="8-Eise-04-decembre-2018IMG_9508-min-scaled"
          />
        </div>
        <div class="photo nine">
          <img
            src="./assets/page-nosProduits/9-Eise-04-decembre-2018IMG_9328-min-scaled.jpg"
            alt="9-Eise-04-decembre-2018IMG_9328-min-scaled"
          />
        </div>
      </div>
      <div class="colonne">
        <div class="photo ten">
          <img
            src="./assets/page-nosProduits/10-Eise-04-decembre-2018IMG_9610-min-scaled.jpg"
            alt="10-Eise-04-decembre-2018IMG_9610-min-scaled"
          />
        </div>
        <div class="photo eleven">
          <img
            src="./assets/page-nosProduits/11-Eise-04-decembre-2018IMG_9486-min-scaled.jpg"
            alt="11-Eise-04-decembre-2018IMG_9486-min-scaled"
          />
        </div>
        <div class="photo eleven">
          <img
            src="./assets/page-nosProduits/9-Eise-04-decembre-2018IMG_9328-min-scaled.jpg"
            alt="11-Eise-04-decembre-2018IMG_9486-min-scaled"
          />
        </div>
      </div>
    </div>

    <p class="paragraphe-centre">
      “La gastronomie est l'art d'utiliser la nourriture pour créer le bonheur.”
      <br />Charles Monselet
    </p>
  </div>
</template>

<script>
export default {
  name: "nos-produits",
};
</script>

<style>
.titre-nos-produits {
  /* height: 16vh; */
  background-color: #cd2428;
  color: #faf5d0;
  padding: 3rem;
  /* position: relative; */
  display: flex;
  flex-direction: row;
}
.moitie {
  width: 50%;
}
.album {
  display: flex;
  flex-direction: row;
  /* flex-wrap: nowrap; */
  flex: 1;
  width: 100%;
  /* column-gap: 1em; */
  /* box-sizing: border-box; */
  justify-content: flex-start;
}
.colonne {
  display: flex;
  flex-direction: column;
  padding: 0.6rem;
  width: 25%;
}
.photo {
  padding: 0.5rem 0;
}
.photo img {
  width: 100%;
  /* object-fit: fill; */
}
/* .album {
  display: grid;
  grid-template-columns: repeat(4, 1fr);
  grid-gap: 1rem;
  width: 100%;
  flex-basis: auto;
  position: relative; 
}

.photo img {
  width: 100%;
  object-fit: fill;
} */

/* .one {
  grid-column: 1 / 2;
  grid-row: 1;
}
.two {
  grid-column: 1 / 2;
  grid-row: 2;
}
.three {
  grid-column: 1 / 2;
  grid-row: 3;
}
.four {
  grid-column: 2 / 3;
  grid-row: 1;
}
.five {
  grid-column: 2 / 3;
  grid-row: 2;
}
.six {
  grid-column: 2 / 3;
  grid-row: 3;
}
.seven {
  grid-column: 3/4;
  grid-row: 1;
}
.height {
  grid-column: 3/4;
  grid-row: 2;
}
.nine {
  grid-column: 3/4;
  grid-row: 3;
}
.ten {
  grid-column: 4/5;
  grid-row: 1;
}
.eleven {
  grid-column: 4/5;
  grid-row: 2;
} */
</style>