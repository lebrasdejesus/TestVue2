<script>
export default {
    name: 'page-accueil',
}
</script>

<template>
    <div>
        <div class="fjord">
        </div>
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
            <div class="petitesimages">

            </div>
            <div class="partietexte">
                <h2>L’histoire des Laksøn</h2>
                <br>
                <h3>Des restaurants à Lille et Rouen</h3>
                <br>
                <p class="textenoir">
                    Les produits Laksøn sont uniques. C'est petit à petit que nous nous sommes tournés vers le Grand Nord.
                    Guidés par la passion et l'authenticité, c'est la bas que nous avons trouvé et sélectionné des produits
                    d'une qualité exceptionnelle. Rares, précieux.
                    <br><br>
                    Traçables, avec un contrôle complet de la filière, préservés par les immensités froides, nos produits
                    sont préparés dans la pure tradition des recettes scandinaves. Un savoir-faire qui se transmet de
                    génération en génération et qui donne aux produits Laksøn ce goût si particulier des choses vraies.
                    <br><br>
                    Chacun de nos produits a une histoire qui lui confère une aura supplémentaire. Laissez vous guider...</p>
                    <br><br>
                    <p class="bold">
                        Bon voyage en terre inconnue !
                    </p>
                
                <div class="boutonblanc coutourrouge">RÉSERVER UNE TABLE</div>
            </div>
        </div>
    </div>
</template>

<style>
.fjord {
    width: 100%;
    height: 100vh;
    box-sizing: border-box;
    background-image: url('./assets/homepage/shutterstock_209912017.jpg');
    background-repeat: no-repeat;
    background-attachment: fixed;
    background-origin: border-box;
    /* background-color: rebeccapurple; */
}

/* .image {
    display: block;
    margin: auto;
} */

.englobeurBouton {
    display: flex;
    justify-content: center;
}

.boutonblanc {
    padding: 1rem;
    background-color: #FAF5D0;
    font-size: 1.3rem;
    color: #CD2428;
    font-style: italic;
    margin-top: 2rem;

    transition: all .3s;
    width: fit-content;
}

.decalagebouton1 {
    top: -100px;
    margin-top: 0;
    position: absolute;

}

.boutonblanc:hover {
    background-color: #CD2428;
    color: #FAF5D0;
    cursor: pointer;
    border: 1px #FAF5D0 solid;
}

.boutonrouge {
    padding: 1rem;
    background-color: #CD2428;
    font-size: 1.3rem;
    color: #FAF5D0;
    font-style: italic;
    border: 1px #FAF5D0 solid;
    margin-top: 2rem;
    transition: all .3s;
    width: fit-content;
}
.coutourrouge{
    border: 1px solid #CD2428;
}
.boutonrouge:hover {
    background-color: #FAF5D0;
    font-size: 1.3rem;
    color: #CD2428;
    font-style: italic;
    border: 1px #CD2428 solid;
}

.secondpart {
    height: 22vh;
    background-color: #CD2428;
    color: blanchedalmond;
    padding: 3rem;
    position: relative;
}

.separate {
    border-top: 1px blanchedalmond solid;
    width: 20rem;
    margin: 2rem 0rem;
}

.thirdpart {
    /* height: 50vh; */
    background-color: #FAF5D0;
    color: #CD2428;
    padding: 3rem;
    position: relative;
    display: flex;
    flex-direction: row;
}

p {
    color: #FAF5D0;
    font-size: 1.3rem;
}

.petitesimages {
    width: 50%;
    background-color: blue;
}

.partietexte {
    width: 50%;
    padding-left: 3rem;
    /* height: fit-content; */
}

.textenoir {
    color: black;
    font-size: 1rem;
    line-height: 1.5rem;
}
.bold{
    font-weight: bold;
}
</style>