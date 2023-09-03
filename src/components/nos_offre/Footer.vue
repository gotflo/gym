<template>
    <div id="Footer">
        <div class="container">
            <div class="row">
                <div class="col-4">
                    <h2>GETFIT</h2>
                    <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis soluta, inventore sequi nam
                        expedita voluptas. Rerum praesentium provident quisquam repudiandae
                    </p>
                </div>
                <div class="col-4">
                    <div class="iconContainer">
                        <div class="row">
                            <i class="bi bi-facebook"></i>
                        </div>
                        <div class="row">
                            <i class="bi bi-instagram"></i>
                        </div>
                        <div class="row">
                            <i class="bi bi-twitter"></i>
                        </div>
                        <div class="row">
                            <i class="bi bi-whatsapp"></i>
                        </div>
                    </div>
                </div>

                <div class="col-4">
                    <div class="row">
                        <img src="./../../assets/gallery1.jpg" alt="box" class="gallery">
                        <img src="./../../assets/gallery2.jpg" alt="box" class="gallery">
                    </div>
                    <div class="row">
                        <img src="./../../assets/gallery3.jpg" alt="box" class="gallery">
                        <img src="./../../assets/gallery4.jpg" alt="box" class="gallery">
                    </div>
                </div>
            </div>
            <div class="copyright">
                <h7>© Copyright
                    <a style="text-decoration:none; color: #000330;" href="http://gotflo.site/">
                        Gotflo</a>. All
                    Rights Reserved
                </h7>
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: "FooterPage",
    setup() {
        return {}
    }
}
</script>

<style scoped>
p {
    text-align: start;
}

.gallery {
    padding: 2px;
    width: 150px;
    height: 100px;
}


.copyright {
    padding-top: 12px;
    padding-bottom: -20px;
}

.bi {
    font-size: 2.1em;
    cursor: pointer;
    padding: 2px;
}

.iconContainer {
    width: 10px;
    /* padding-right: 100px; */
    padding-left: 100px;
}

.col-4 {
    text-align: start;
}

.container {
    padding: 3%;
}

/* Train rouge en bas du texte NOS OFFRES */
h2 {
    color: red;
    font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
    padding-bottom: 12px;
}
</style>
