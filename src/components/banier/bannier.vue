<template>
    <div class="vh-100 overflow-hidden" id="bannier">
        <NavBar />
        <div class="vh-100 overflow-hidden decorationdiv"></div>
        <div class="BannierContainer ">
            <h1 class="h1text">Il est temps de se mettre en <span>forme</span></h1>
            <h5 class="h5text">Le succès vient généralement à ceux qui sont <br />trop occupés pour le chercher.</h5>
            <br />
            <div class="col">
                <button type="button" class="btn btn-danger">EXPLORER PLUS</button>
                <button type="button" class="btn btn-contact" style="margin-left: 20px;">CONTACTER</button>
            </div>
        </div>
    </div>
</template>

<script>
import NavBar from '../navbar/navbar.vue'

export default {
    name: "BannierVue",
    components: {
        NavBar,
    },
    setup() {
        return {}
    }
}
</script>

<style scoped>
#bannier {
    background: url("../../assets/bg-image.jpg") rgba(77, 67, 67, 0.705);
    background-blend-mode: multiply;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
}

.h1text span {
    color: #d80000;
}



.btn-danger {
    background: #d80000;
    border-radius: 0px;
}

.btn-contact {
    background: rgba(49, 49, 49, 0.301);
    border-radius: 0px;
    color: white;
    border: 1px solid white;
}

.h1text {
    text-transform: uppercase;
    color: white;
    font-size: 2rem;
    text-align: center;
}

.h5text {
    color: #b3b3b3;
}

.decorationdiv {
    background-color: rgba(71, 62, 62, 0.274);
}

.BannierContainer {
    /* /* top: 50%; */
    color: white;
    /* position: absolute;
    left: 25%;
    margin: -25px 0 0 -25px; */
}
</style>