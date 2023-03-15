<template>
    <section>
        <div class="container">
            <h1>LET'S TALK ABOUT WORK</h1>
            <p>A wonderful serenity has taken possession Far far away, behind the word mountains.</p>
            <button class="about__green-button">GET STARTED</button>
        </div>
        <div class="container__social">
            <img src="/images/logotype-2-139x23.png" alt="">
            <ul class="social">
                <li><img class="icons" src="/icons8-instagram.svg" alt=""></li>
                <li><img class="icons" src="/icons8-linkedin.svg" alt=""></li>
                <li><img class="icons" src="icons8-facebook.svg" alt=""></li>
                <li><img class="icons" src="icons8-twitter.svg" alt=""></li>
            </ul>
        </div>
        <nav>
            <ul class="navigation">
                <li v-for="item in menuItems" :key="item.id">
                    <a :href="item.link">{{ item.name }}</a>
                </li>
            </ul>
        </nav>
        <div class="copyright">
            <p>Terms of use
                <br>
                Privacy Environmental Policy
            </p>
            <p>
                Copyright © 2023 Phlox Consulting. All Rights Reserved.
            </p>
        </div>
    </section>
</template>

<script>
export default {
    data() {
        return {
            menuItems: [
                { id: 1, name: 'HOME', link: '/' },
                { id: 2, name: 'ABOUT', link: '/about' },
                { id: 3, name: 'PROJECTS', link: '/projects' },
                { id: 4, name: 'SERVICES', link: '/services' },
                { id: 5, name: 'BLOG', link: '/blog' },
                { id: 6, name: 'CONTACT', link: '/contact' },
            ],
        };
    },
};
</script>


<style lang="scss" scoped>
.copyright {
    color: #5D5C6E;
    font-weight: 100;
    display: flex;
    align-items: flex-end;
    justify-content: space-between;
    padding-top: 25px;
    padding-bottom: 25px;
}

.container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    color: white;
    text-align: center;
    background-image: url(/images/business-people-working-together-on-project-and-B3MZ4TX.jpg);
    background-position: center;
    min-height: 400px;
}

.container__social {
    padding-top: 100px;
    padding-bottom: 25px;
    background-color: #151838;
    display: flex;
    align-items: center;
}

.navigation {
    padding-top: 25px;
    padding-bottom: 25px;
    display: flex;
    list-style: none;
    justify-content: space-around;
    color: #5D5C6E;
    border-top: 1px solid #5D5C6E;
    border-bottom: 1px solid #5D5C6E;

    li {
        a {
            &:hover {
                color: #F81D39;
            }
        }
    }
}

section {
    background-color: #151838;
}

h1 {
    padding-bottom: 15px;
}

p {
    padding-bottom: 25px;
}

.about__green-button {
    padding: 20px 30px;
    background-color: #151838;
    color: #fff;
    border: none;
    cursor: pointer;
    font-size: 18px;

    &:hover {
        background-color: #39FFBF;
        color: #fff;
    }
}

.icons {
    max-width: 30px;
}

.social {
    list-style: none;
    display: flex;
}

li {
    padding: 15px;
}
</style>