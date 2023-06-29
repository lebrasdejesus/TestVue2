<script>
export default {
    name: 'NavB',
}
</script>

<template>
    <div class="navbar">
        <div class="menulogo"><a href="#/"><img class="logo" alt="Vue logo" src="../assets/navbar/Lakson-logo.png"></a>
        </div>
        <div></div>
        <div></div>
        <div></div>
        <div class="menu"><a href="#/contenu1">Accueil</a></div>
        <div class="menu"><a href="#/contenu2">Nos restaurants</a></div>
        <div class="menu"><a href="#/contenu3">Nos produits</a></div>
        <div class="menu"><a href="#/contenu4">Réservations</a></div>
    </div>
</template>

<style>

.navbar {
    background-color: #CD2428;
    border: 1px solid #FAF5D0;
    height: 3.5rem;
    display: grid;
    grid-template-columns: 2fr  2fr 2fr 2fr 2fr 2fr 2fr 2fr;
    /* margin: 1rem; */
    color: #FAF5D0;
    font-size: 1.2rem;
    font-family: 'Cormorant Garamond', serif;
    font-weight: 100;
}

.navbar>div {
}

.logo {
    max-height: 1.2rem;
    max-width: 80%;
    padding: 0px 0px;
}

.menu {
    display: flex;
    justify-content: center;
    align-items: center;
}

.menulogo {
    display: flex;
    justify-content: left;
    align-items: center;
    padding-left: 1rem;
}

a {
    text-decoration: none;
    color: inherit;
}</style>