<template>
    <section class="hero">
        <div class="left__side">
            <div class="hero__container">
                <h2 class="hero__subtitle">{{ subtitle }}</h2>
                <h1 class="hero__title">{{ title }}</h1>
                <button class="hero__cta">{{ ctaText }}</button>
            </div>
        </div>
        <div class="lato__destro">
            <img src="/images/portrait-of-young-architect-woman-on-meeting-KFZCE3A.jpg" alt="">
        </div>
    </section>
</template>
  
<script>
export default {
    data() {
        return {
            title: "THE BEST BUSINESS CONSULTING",
            subtitle: "ALWAYS THE BEST WAY YOU NEED IT",
            ctaText: "READ MORE"
        };
    }
};
</script>


  
<style lang="scss" scoped>
.hero {
    background-color: #1F1838;
    display: flex;
}

img {
    display: block;
}

.left__side {
    padding-left: 25px;
}

.hero__container {
    padding-top: 200px;
}

.hero__title {
    font-size: 48px;
    font-weight: bold;
    color: #fff;
}

.hero__subtitle {
    font-size: 24px;
    font-weight: bold;
    color: #fff;
    margin-top: 20px;
}

.hero__cta {
    background-color: #fff;
    color: #000;
    font-size: 18px;
    font-weight: bold;
    text-transform: uppercase;
    border: none;
    padding: 15px 30px;
    margin-top: 40px;
    cursor: pointer;
    transition: all 0.2s ease-in-out;

    &:hover {
        background-color: #000;
        color: #fff;
    }
}
</style>