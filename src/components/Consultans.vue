<template>
    <div class="container">
        <h2 class="title__section">OUR CONSULTANS CAN HELP YOU</h2>
        <div class="title__section-line"></div>
        <div class="cards-wrapper">
            <div class="card">
                <img src="/line-graph.svg" alt="">
                <div class="text">
                    <h4>STATISTICAL CONSULTING</h4>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a</p>
                </div>
            </div>
            <div class="card">
                <img src="/shout.svg" alt="">
                <div class="text">
                    <h4>DIGITAL CONSULTING</h4>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a</p>
                </div>
            </div>
        </div>
        <div class="cards-wrapper">
            <div class="card">
                <img src="/path-13.svg" alt="">
                <div class="text">
                    <h4>BANKING CONSULTING</h4>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a</p>
                </div>
            </div>
            <div class="card">
                <img src="/target.svg" alt="">
                <div class="text">
                    <h4>ENTERPRISE CONSULTING</h4>
                    <p>When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable
                        foliage of my trees, and but a</p>
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
.title__section {
    margin: 50px 50px;
}

.container {
    max-width: 1200px;
}

.cards-wrapper {
    display: flex;
}

.card {
    flex-basis: 50%;
    display: flex;
    padding: 25px;
}

img {
    background-color: #F81D39;
    aspect-ratio: 1;
    border-radius: 50%;
    padding: 10px;
    margin-right: 15px;
}
</style>
  