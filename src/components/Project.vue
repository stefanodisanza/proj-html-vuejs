<template>
    <div class="section">

        <body>
            <div class="conteiner__top">
                <div class="text">
                    <h4 class="title">PROJECT</h4>
                    <h1 class="subtitle">OUR EXPERT TRUSTED CONSULTANTS HELP CLIENTS</h1>
                </div>
                <div class="arrow-container">
                    <div class="arrow-button left-arrow"></div>
                    <div class="arrow-button right-arrow"></div>
                </div>
            </div>
            <div class="container">
                <div class="image-container">
                    <img class="image" src="/images/DRY-1-790x592.jpg" alt="Immagine 1">
                    <img class="image" src="/images/221bf0b7-8134-43bb-936a-5acbe42db64a-790x592.jpg" alt="Immagine 2">
                    <img class="image" src="/images/z1el4c4p-790x592.jpg" alt="Immagine 3">
                </div>

            </div>
        </body>
    </div>
</template>

<script>
export default {

}
</script>

<style lang="scss" scoped>
.section {
    background-color: #1F1838;
    color: white;
}

.conteiner__top {
    display: flex;
    padding-top: 150px;
}


/* Stile per il contenitore principale */
.container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    margin-top: 50px;
    padding-bottom: 100px;
}

/*Stile per il conteiner dei testi */
.text {
    margin-left: 50px;
    margin-right: 50px;
    display: flex;
    flex-direction: column;


}



/* Stile per il titolo */
.title {
    padding: 20px 0;
}

/* Stile per il contenitore delle immagini */
.image-container {
    display: flex;
    flex-direction: row;
    justify-content: center;
    align-items: center;
    margin-top: 20px;
}

/* Stile per le immagini */
.image {
    width: 300px;
    height: 200px;
    object-fit: cover;
    margin-right: 20px;
}

/* Stile per il contenitore dei pulsanti delle frecce */
.arrow-container {
    display: flex;
    justify-content: space-between;
    align-items: center;
    width: 100%;
    margin-top: 20px;
}

/* Stile per i pulsanti delle frecce */
.arrow-button {
    display: flex;
    justify-content: center;
    align-items: center;
    width: 50px;
    height: 50px;
    background-color: #362d59;
    border-radius: 5px;
    cursor: pointer;
}

/* Stile per l'icona della freccia destra */
.arrow-button.right-arrow::after {
    content: "\2192";
    font-size: 24px;
    color: #fff;
}

/* Stile per l'icona della freccia sinistra */
.arrow-button.left-arrow::after {
    content: "\2190";
    font-size: 24px;
    color: #fff;
}
</style>
