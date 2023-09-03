<template>
    <div id="NosClasses">
        <h2>CLASSES</h2>
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <div class="card">
                        <img src="./../../assets/box.jpg" alt="box" class="card-img-top">
                        <div class="card-overlay">
                            <p>Texte sur l'image</p>
                        </div>
                    </div>
                </div>
                <div class="col-4">
                    <div class="card">
                        <img src="./../../assets/exercice.jpg" alt="box" class="card-img-top">
                        <div class="card-overlay">
                            <p>Texte sur l'image</p>
                        </div>
                    </div>
                </div>
                <div class="col-4">
                    <div class="card">
                        <img src="./../../assets/velo.jpg" alt="box" class="card-img-top">
                        <div class="card-overlay">
                            <p>Texte sur l'image</p>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "NosClasses",
    setup() {
        return {}
    }
}
</script>

<style scoped>
h2 {
    margin-top: 30px;
    color: black;
    position: relative;
}

.card {
    margin-top: 5%;
    margin-bottom: 20%;
    position: relative;
    box-shadow: 0px 4px 6px rgba(0, 0, 0, 0.1);
    transition: transform 0.3s, box-shadow 0.3s;
}

.card:hover {
    /* Lorsqu'on survole la carte */
    transform: translateY(-5px);
    /* Déplacer légèrement vers le haut */
    box-shadow: 0px 8px 10px rgba(0, 0, 0, 0.2);
    /* Augmenter l'ombre */
}

.card-overlay {
    position: absolute;
    top: 0;
    left: 0;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;
    opacity: 0;
    transition: opacity 0.3s;
    cursor: pointer;
}

.card:hover .card-overlay {
    /* Lorsqu'on survole la carte */
    opacity: 1;
    /* Afficher le texte au survol */
}

.card .card-overlay {
    opacity: 1;
    /* Afficher lors du survol */
}

p {
    margin-top: 50%;
    margin-left: -40%;
}

/* Train rouge en bas du texte NOS OFFRES */
h2::after {
    content: "";
    display: block;
    width: 90px;
    height: 3px;
    background-color: red;
    position: absolute;
    left: 51%;
    transform: translateX(-72%);
}
</style>
