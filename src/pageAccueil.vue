<script>
export default {
  name: "page-accueil",
};
</script>

<template>
  <div>
    <div class="fjord"></div>

    <div class="secondpart">
      <div class="englobeurBouton">
        <div class="boutonblanc decalagebouton1">VOIR NOS RESTAURANTS</div>
      </div>
      <h2>LAKSØN - Maison Scandinave</h2>
      <div class="separate"></div>
      <p>Spécialités Nordiques et de poissons frais depuis 1987</p>
      <div class="englobeurBouton">
        <div class="boutonrouge">RÉSERVER UNE TABLE</div>
      </div>
    </div>

    <div class="thirdpart">
      <div class="divpetitesimages">
        <div class="sousdivpetitesimages">
          <img
            class="petitesimages ptimg1"
            src="./assets/homepage/Cour-interieur-lakson-lille.jpg.jpg"
            alt="cour intérieure Lille"
          />
        </div>
        <div class="sousdivpetitesimages">
          <img
            class="petitesimages ptimg2"
            src="./assets/homepage/Boutique-Lakson-Lille-Photo-1.jpg"
            alt="Boutique Lille"
          />
        </div>
      </div>
      <div class="partietexte">
        <h2>L’histoire des Laksøn</h2>
        <br />
        <h3>Des restaurants à Lille et Rouen</h3>
        <br />
        <p class="textenoir">
          Les produits Laksøn sont uniques. C'est petit à petit que nous nous
          sommes tournés vers le Grand Nord. Guidés par la passion et
          l'authenticité, c'est la bas que nous avons trouvé et sélectionné des
          produits d'une qualité exceptionnelle. Rares, précieux.
          <br /><br />
          Traçables, avec un contrôle complet de la filière, préservés par les
          immensités froides, nos produits sont préparés dans la pure tradition
          des recettes scandinaves. Un savoir-faire qui se transmet de
          génération en génération et qui donne aux produits Laksøn ce goût si
          particulier des choses vraies.
          <br /><br />
          Chacun de nos produits a une histoire qui lui confère une aura
          supplémentaire. Laissez vous guider...
        </p>
        <br /><br />
        <p class="bold">Bon voyage en terre inconnue !</p>
        <div class="boutonblanc coutourrouge">RÉSERVER UNE TABLE</div>
      </div>
    </div>

    <div class="fourthpart">
      <div class="partietexte">
        <h2>Nos restaurants</h2>
        <br />
        <p>Lille - Rouen - Halles Agrivin (Rouen)</p>
        <br />
      </div>
      <div class="conteneur-accordeon">
        <div class="sous-conteneur-accordeon">
          <img
            class="img-accordeon"
            src="./assets/homepage/Entree-Lakson-Rouen.jpg"
            alt="Rouen"
          />
        </div>
        <div class="sous-conteneur-accordeon">
          <img
            class="img-accordeon"
            src="./assets/homepage/Lakson-de-Lille.jpg"
            alt="Lille"
          />
        </div>
        <div class="sous-conteneur-accordeon">
          <img
            class="img-accordeon"
            src="./assets/homepage/Photos-fictives-des-restaurants-1.jpg"
            alt="Rouen bis"
          />
        </div>
      </div>
    </div>
  </div>
</template>

<style>
.fjord {
  width: 100%;
  height: 100vh;
  box-sizing: border-box;
  background-image: url("./assets/homepage/shutterstock_209912017.jpg");
  background-repeat: no-repeat;
  background-attachment: fixed;
  background-origin: border-box;
  /* background-color: rebeccapurple; */
}

.englobeurBouton {
  display: flex;
  justify-content: center;
}

.boutonblanc {
  padding: 1rem;
  background-color: #faf5d0;
  font-size: 1.3rem;
  color: #cd2428;
  font-style: italic;
  margin-top: 2rem;
  transition: all 0.3s;
  width: fit-content;
}

.decalagebouton1 {
  top: -100px;
  margin-top: 0;
  position: absolute;
}

.boutonblanc:hover {
  background-color: #cd2428;
  color: #faf5d0;
  cursor: pointer;
  border: 1px #faf5d0 solid;
}

.boutonrouge {
  padding: 1rem;
  background-color: #cd2428;
  font-size: 1.3rem;
  color: #faf5d0;
  font-style: italic;
  border: 1px #faf5d0 solid;
  margin-top: 2rem;
  transition: all 0.3s;
  width: fit-content;
}
.coutourrouge {
  border: 1px solid #cd2428;
}
.boutonrouge:hover {
  background-color: #faf5d0;
  font-size: 1.3rem;
  color: #cd2428;
  font-style: italic;
  border: 1px #cd2428 solid;
}

.secondpart {
  height: 16vh;
  background-color: #cd2428;
  color: #faf5d0;
  padding: 3rem;
  position: relative;
}

.separate {
  border-top: 1px #faf5d0 solid;
  width: 20rem;
  margin: 2rem 0rem;
}
h2 {
  font-family: "Montserrat", sans-serif;
  font-style: italic;
  font-weight: 400;
  font-size: 2rem;
}
.thirdpart {
  /* height: 50vh; */
  background-color: #faf5d0;
  color: #cd2428;
  padding: 3rem;
  position: relative;
  display: flex;
  flex-direction: row;
}

p {
  color: #faf5d0;
  font-size: 1.3rem;
}

.divpetitesimages {
  position: relative;
  width: 50%;
  display: flex;
  justify-content: center;
  /* align-items: center; */
  /* border: 1px solid blue; */
}
.sousdivpetitesimages {
  position: relative;
  width: 40%;
  display: flex;
  justify-content: center;
  align-items: center;
  /* border: 1px solid rgb(20, 75, 22); */
}
.petitesimages {
  border: #cd2428 solid 3px;
  position: absolute;
  max-width: 100%;
}
.ptimg1 {
  opacity: 1;
  position: absolute;
  display: block;
  transform: translate(5%, -5%);
}
.ptimg2 {
  position: absolute;
  /* bottom: 10%;
  left: 20%; */
  /* margin-bottom: -38%;
  margin-left: 30%; */
  display: block;
  z-index: 1;
  transform: translate(-5%, 5%);
}
.partietexte {
  width: 50%;
  padding-left: 3rem;
}

.textenoir {
  color: black;
  font-size: 1rem;
  line-height: 1.5rem;
}
.bold {
  font-weight: bold;
}

.fourthpart {
  height: 40rem;
  background-color: #bc8889;
  color: #faf5d0;
  padding: 3rem;
  /* position: relative; */
  display: flex;
  flex-direction: column;
}
.texteblanc {
  font-size: 1rem;
  line-height: 1.5rem;
}
.conteneur-accordeon {
  display: flex;
  flex-direction: row;
  position: relative;
  width: 100%;
  max-height: 85%;
  /* height: 33rem; */
  /* justify-content: top;
  align-items: start; */
  border: solid 1px #24cd35;
  /* overflow: hidden; */
}
.sous-conteneur-accordeon {
  position: relative;
  width: 33.33%;
  max-height: 100%;
  /* display: flex; */
  /* flex-direction: row; */
  justify-content: top;
  align-items: center;
  border: solid 2px #ba41ea;
  /* overflow: hidden; */
}
.img-accordeon {
  /* position: absolute; */
  /* max-width: 100%;
  max-height: 100%;
  overflow: hidden; */
  width: 100%;
  height: 100%;
  object-fit: cover;
}
</style>