<template>
    <div class="container">
        <div class="text">
            <h4>BLOG</h4>
            <h1>BLOG
                THE RECENT NEWS YOU MUST READ IT</h1>
            <button class="about__green-button">VIEW ALL</button>
        </div>
        <div class="container__cards">
            <div class="card">
                <img src="/images/startup-business-people-and-strategy-board-PAJ3P9K-1390x1042.jpg" alt="">
                <div class="card__text">
                    <h5>july 4, 2019 by paul</h5>
                    <h3>Canadian Consulting Firm acquired by UK Giant</h3>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a ...</p>
                </div>
            </div>
            <div class="card">
                <img src="/images/business-people-working-together-on-project-and-5FHSKBL-1390.jpg" alt="">
                <div class="card__text">
                    <h5>july 4, 2019 by paul</h5>
                    <h3>JCanadian Consulting Firm acquired by UK Giant</h3>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a ...</p>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss" scoped>
img {
    max-width: 100%;
    display: block;
}

.container {
    padding-top: 150px;
    padding-bottom: 200px;
    background-color: #1F1838;
}

.text {
    position: relative;
}

h4 {
    color: white;
    text-align: start;
    padding-bottom: 25px;
    padding-left: 25px;
}

h1 {
    color: white;
    text-align: start;
    padding-left: 25px;
}

.about__green-button {
    position: absolute;
    bottom: 0px;
    right: 15px;
    padding: 20px 30px;
    background-color: #39FFBF;
    color: black;
    border: none;
    cursor: pointer;
    font-size: 18px;

    &:hover {
        background-color: #F81D39;
        color: #fff;
    }
}

.container__cards {
    display: flex;
    justify-content: space-between;
}

.card {
    position: relative;
    flex-basis: 50%;
    width: 50%;
    height: auto;
    overflow: visible;
    margin: 15px;
}

.card__text {
    position: absolute;
    bottom: -55px;
    right: 0px;
    background-color: white;
    color: black;
    padding: 25px 50px;
    box-sizing: border-box;
    width: 65%;
    text-align: left;
}

.card__text h3 {
    margin-top: 0;
}

.card__text p {
    margin-bottom: 0;
}

@media only screen and (max-width: 768px) {
    .card__text {
        width: 100%;
        max-width: none;
    }
}
</style>