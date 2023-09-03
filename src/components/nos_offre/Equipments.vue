<template>
    <div class="vh-100 overflow-hidden" id="Equipments">
        <div class="container">
            <h2>Meilleurs <span>équipements</span> <br />et <span>entraîneurs</span> de fitness</h2>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Perferendis soluta, inventore sequi nam expedita
                voluptas. Rerum praesentium provident quisquam repudiandae
            </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "EquipmentsPage",
    setup() {


        return {}
    }
}
</script>

<style scoped>
#Equipments {
    background: url("../../assets/equipment.jpg") rgba(53, 53, 53, 0.445);
    background-blend-mode: multiply;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
}

.container {
    width: 300px;
    background: rgba(53, 53, 53, 0.692);
    color: white;
    margin-left: 10%;
    margin-right: auto;
    padding: 20px;
}

.container:hover {
    background: rgb(15, 15, 15);
    cursor: pointer;
    border: 1px solid #d80000;
}

.container {
    transition: background-color 0.3s ease-in-out, opacity 0.3s ease-in-out;
}

h2 {
    text-transform: uppercase;
    font-size: 1rem;
    text-align: start;
}

p {
    font-weight: 100;
    color: rgba(255, 255, 255, 0.596);
    text-align: justify;
}

span {
    color: #d80000;
}
</style>