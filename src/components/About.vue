<template>
    <section class="about">
        <div class="left__side">
            <img src="/images/business-people-working-together-on-project-and-5FHSKBL.jpg" alt="">
        </div>
        <div class="right__side">
            <div class="about__container">
                <h4 class="about__subtitle">{{ subtitle }}</h4>
                <h1 class="about__title">{{ title }}</h1>
                <p class="about__text">{{ text }}</p>
            </div>
        </div>

    </section>
    <div class="about__green">
        <div class="about__green-text">
            <h2>WE HELP TO DELIVER THE BUSINESS CASE</h2>
            <p>When, while lovely valley teems with vapour around meand meridian sun strikes the upper impenetrable foliage
                of my trees, and but a thousand unknown</p>
        </div>
        <button class="about__green-button">GET STARTED</button>
    </div>
</template>

<script>

export default {
    data() {
        return {
            title: "WE MAKE YOUR STRATEGY WORK",
            subtitle: "ABOUT US",
            text: "When, while lovely valley teems with vapour around meand eridian sun strikes the upper impenetrable foliage of my trees, and but a thousand unknown plants are noticed when I hear the buzz of the little world among the stalks,and grow familiar indescribable forms of the insects .and flies, then I feel the presence of the Almighty . "
        };
    }

}
</script>

<style lang="scss" scoped>
.about {
    background-color: #1F1838;
    display: flex;
}

.about__green {
    display: flex;
    justify-content: space-between;
    padding: 100px;
    align-items: center;
    background-color: #39FFBF;
    position: relative;
}

.about__green-text {
    margin-right: 150px;
    display: flex;
    justify-content: space-between;
}

h2 {
    margin-right: 100px;
}

.about__green-button {
    position: absolute;
    bottom: 0px;
    right: 0px;
    padding: 20px 30px;
    background-color: #F81D39;
    color: #fff;
    border: none;
    cursor: pointer;
    font-size: 18px;
}

.about__subtitle {
    margin-bottom: 20px;
}

.about__title {
    margin-bottom: 20px;
}

img {
    display: block;
}

.right__side {
    padding-left: 25px;
}

.about__container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: flex-start;
    text-align: left;
    margin: 0 auto;
    max-width: 800px;
    height: 100%;
    color: #fff;
    padding: 20px;
}
</style>
