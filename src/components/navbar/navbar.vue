<template>
    <nav class="navbar navbar-expand-lg navbar-dark fixed-top"
        :class="{ 'bg-transparent': !isScrolled, 'bg-black': isScrolled }">
        <div class="container">
            <a class="navbar-brand" href="#">GETFIT</a>
            <button class="navbar-toggler shadow-none border-0" type="button" data-bs-toggle="collapse"
                data-bs-target="#navbarSupportedContent" aria-controls="navbarSupportedContent" aria-expanded="false"
                aria-label="Toggle navigation">
                <span class="navbar-toggler-icon"></span>
            </button>
            <div class="collapse navbar-collapse" id="navbarSupportedContent">
                <ul class="navbar-nav me-auto mb-2 mb-lg-0 list-inline mx-auto justify-content-center">
                    <li class="nav-item" :class="{ 'active': activeTab === 'ACCUEIL' }">
                        <a class="nav-link" aria-current="page" href="#bannier" @click="setActiveTab('ACCUEIL')">ACCUEIL</a>
                    </li>
                    <li class="nav-item" :class="{ 'active': activeTab === 'NOS OFFRES' }">
                        <a class="nav-link" aria-current="page" href="#NosOffres" @click="setActiveTab('NOS OFFRES')">NOS
                            OFFRES</a>
                    </li>
                    <li class="nav-item" :class="{ 'active': activeTab === 'CLASSES' }">
                        <a class="nav-link" aria-current="page" href="#NosClasses"
                            @click="setActiveTab('CLASSES')">CLASSES</a>
                    </li>
                    <li class="nav-item" :class="{ 'active': activeTab === 'FORMATEURS' }">
                        <a class="nav-link" aria-current="page" href="#NosFormateurs"
                            @click="setActiveTab('FORMATEURS')">FORMATEURS</a>
                    </li>
                    <li class="nav-item" :class="{ 'active': activeTab === 'BLOG' }">
                        <a class="nav-link" aria-current="page" href="#" @click="setActiveTab('BLOG')">BLOG</a>
                    </li>
                    <li class="nav-item" :class="{ 'active': activeTab === 'CONTACTEZ-NOUS' }">
                        <a class="nav-link" aria-current="page" href="#ContactUS"
                            @click="setActiveTab('CONTACTEZ-NOUS')">CONTACTEZ-NOUS</a>
                    </li>
                </ul>
            </div>
        </div>
    </nav>
</template>

<script>
export default {
    name: "NavBar",
    data() {
        return {
            activeTab: "ACCUEIL",
            isScrolled: false
        };
    },
    methods: {
        setActiveTab(tab) {
            this.activeTab = tab;
        },
        handleScroll() {
            const NosOffres = document.getElementById('NosOffres');
            if (NosOffres) {
                const rect = NosOffres.getBoundingClientRect();
                this.isScrolled = window.scrollY >= rect.top;
            }
        }
    },
    mounted() {
        window.addEventListener('scroll', this.handleScroll);
        this.handleScroll(); // Appeler dès le début pour s'assurer de l'état initial
    },

    beforeUnmount() {
        window.removeEventListener('scroll', this.handleScroll);
    },
};
</script>

<style  scoped>
.nav-link {
    font-size: 0.8rem;
    font-family: 'Lucida Sans', 'Lucida Sans Regular', 'Lucida Grande', 'Lucida Sans Unicode', Geneva, Verdana, sans-serif;
}

/* Styles pour l'élément actif */
.nav-item.active .nav-link {
    color: white !important;
    text-decoration: solid;
}

/* Barre rouge en bas de l'élément actif */
.nav-item.active .nav-link::after {
    content: "";
    display: block;
    width: 100%;
    height: 3px;
    background-color: red;
}

/* Ajoutez une transition pour le changement de background-color */
.navbar {
    transition: background-color 0.3s ease-in-out, opacity 0.3s ease-in-out;
}

/* Pour le fond noir du navbar après le défilement */
.bg-black {
    background-color: black;
    opacity: 0.9;
    /* Opacité initiale */
}

/* Appliquez une opacité maximale lorsque l'utilisateur défile */
.is-scrolled .bg-black {
    opacity: 1;
}
</style>