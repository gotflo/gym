<template>
    <div class="vh-100 overflow-hidden" id="CalculateBMI">
        <div class="container">
            <h2>Calculez votre <span>BMI</span> </h2>
            <p>L'indice de masse corporelle (IMC) ou Body Mass Index (BMI) indique le rapport entre votre poids et votre
                taille en mètre
            </p>
            <form>
                <div class="form-group">
                    <input type="poids" class="form-control" id="exampleInputPoids" aria-describedby="emailHelp"
                        placeholder="Poids">
                </div>
                <div class="form-group pt-3">
                    <input type="taille" class="form-control" id="exampleInputTaille" placeholder="Taille">
                </div>
                <fieldset disabled>
                    <div class="form-group pt-3 pb-3">
                        <input type="bmi" class="form-control" id="exampleInputBmi" placeholder="BMI" readonly>
                    </div>
                </fieldset>
                <div class="btndiv">
                    <button type="submit" class="btn btn-danger">CALCULER BMI</button>
                </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: "CalculateBMI",
    setup() {


        return {}
    }
}
</script>

<style scoped>
#CalculateBMI {
    background: url("../../assets/CalculateBMI.jpg") rgba(53, 53, 53, 0.445);
    background-blend-mode: multiply;
    background-position: center;
    background-size: cover;
    background-repeat: no-repeat;
    position: relative;
    display: flex;
    justify-content: center;
    align-items: center;
}

.form-control {
    background-color: transparent !important;
}

::placeholder {
    color: #c2c2c29a !important;
}


.btn-danger {
    background: #d80000;
    border-radius: 0px;
}



.container {
    width: 400px;
    background: rgba(53, 53, 53, 0.692);
    color: white;
    margin-right: 10%;
    margin-left: auto;
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
    font-size: 2rem;
    text-align: start;
}

p {
    font-weight: 100;
    color: rgba(255, 255, 255, 0.74);
    text-align: justify;
    font-size: 0.8rem;
}

span {
    color: #d80000;
}
</style>