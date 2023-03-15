<template>
    <div class="text">
        <h4>TESTIMONIAL</h4>
        <h1>WHAT'S THE CUSTOMER SAY ABOUT OUR WORK</h1>
    </div>
    <div class="container">
        <div class="card card1">
            <div class="card-content">
                <p class="paragrafo">When, while lovely valley teems with vapour around meand eridian sun strikes the upper
                    impenetrable
                    foliage
                    of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</p>
                <h3>Vera Duncan</h3>
                <p>Amazon Inc.</p>
            </div>
        </div>
        <div class="card card2">
            <div class="card-content">
                <p class="paragrafo">When, while lovely valley teems with vapour around meand eridian sun strikes the upper
                    impenetrable
                    foliage
                    of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</p>
                <h3>Vera Duncan</h3>
                <p>Amazon Inc.</p>
            </div>
        </div>
        <div class="card card3">
            <div class="card-content">
                <p class="paragrafo">When, while lovely valley teems with vapour around meand eridian sun strikes the upper
                    impenetrable
                    foliage
                    of my trees, and but a thousand unknown plants are noticed by when I hear the buzz of the little .</p>
                <h3>Vera Duncan</h3>
                <p>Amazon Inc.</p>
            </div>
        </div>
    </div>
</template>
  
<script>
export default {};
</script>
  
<style lang="scss" scoped>
.container {
    display: flex;
}

.card {
    flex: 1;
    padding: 50px;
    background-color: white;
    text-align: center;
    transition: background-image 0.1s ease;
    display: flex;
    flex-direction: column;
    height: 100%;
    aspect-ratio: 1/1;
}

.card-content {
    flex-grow: 1;
}

.card1 {
    background-image: url("path/to/image1");
    background-size: cover;
    background-position: center;
}

.card2 {
    background-image: url("path/to/image2");
    background-size: cover;
    background-position: center;
}

.card3 {
    background-image: url("path/to/image3");
    background-size: cover;
    background-position: center;
}

.card:hover {
    background-image: none;
}

.card:hover.card1 {
    background-image: url("/images/oliver-ragfelt-488196-2.jpg");
    color: white;
}

.card:hover.card2 {
    background-image: url("/images/12679.jpg");
    color: white;
}

.card:hover.card3 {
    background-image: url("/images/oliver-ragfelt-488196-unsplash.jpg");
    color: white;
}

.card p:last-child {
    margin-bottom: 0;
}

.text {
    background-color: #1f1838;
    color: white;
}

h4 {
    text-align: center;
    padding-bottom: 25px;
}

h1 {
    text-align: end;
    padding-right: 25px;
    padding-bottom: 50px;
}

.paragrafo {
    padding-bottom: 170px;
}

@media (max-width: 768px) {
    .container {
        flex-direction: column;
    }

    .card {
        width: 100%;
    }
}
</style>