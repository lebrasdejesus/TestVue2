<template>
  <div>
    <div class="titre-nos-produits">
      <div class="moitie">
        <h2>LAKSØN - Maison Scandinave à Lille & Rouen</h2>
        <p>Gastronomie suédoise, norvégienne et danoise​</p>
      </div>
      <div class="moitie"></div>
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
</style>