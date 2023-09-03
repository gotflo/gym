<template>
    <div class="vh-100 overflow-hidden" id="ContactUS">
        <div class="container">
            <h2>CONTACTEZ - <span>NOUS</span> </h2>
            <form>
                <div class="form-group">
                    <input type="name" class="form-control" id="exampleInputName" placeholder="Votre Nom">
                </div>
                <div class="form-group pt-3">
                    <input type="email" class="form-control" id="exampleInputEmail" placeholder="Votre Email"
                        aria-describedby="emailHelp">
                </div>
                <div class="form-group pt-3 pb-3">
                    <textarea class="form-control" id="exampleFormControlTextarea1" placeholder="Message"
                        rows="4"></textarea>
                </div>
                <div class="btndiv">
                    <button type="submit" class="btn btn-danger">ENVOYER</button>
                </div>
            </form>
        </div>
    </div>
</template>

<script>
export default {
    name: "ContactUS",
    setup() {


        return {}
    }
}
</script>

<style scoped>
#ContactUS {
    background: url("../../assets/contactus.jpg") rgba(53, 53, 53, 0.445);
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