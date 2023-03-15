<template>
    <header class="header">
        <div class="header__container">
            <!-- logo e navbar -->
            <img class="header__logo" src="/images/logotype.png" alt="">
            <nav class="header__nav">
                <ul>
                    <li v-for="link in links" :key="link.id">
                        <a :href="link.url" :class="{ 'nav-link': true }">{{ link.label }}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    data() {
        return {
            title: 'Phlox Consulting',
            links: [
                { id: 1, label: 'Home', url: '/' },
                { id: 2, label: 'About', url: '/about' },
                { id: 3, label: 'Projects', url: '/projects' },
                { id: 4, label: 'Services', url: '/services' },
                { id: 5, label: 'Blog', url: '/blog' },
                { id: 6, label: 'Contact', url: '/contact' },
            ],
        };
    },
    mounted() {
        window.addEventListener('scroll', this.handleScroll);
    },
    beforeDestroy() {
        window.removeEventListener('scroll', this.handleScroll);
    },
    methods: {
        handleScroll() {
            const navbar = document.querySelector('.header');
            const scrollPosition = window.scrollY;

            if (scrollPosition > 0) {
                navbar.classList.add('hide-nav');
            } else {
                navbar.classList.remove('hide-nav');
            }
        },
    },
};
</script>

<style lang="scss" scoped>
.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
    overflow: hidden;

    &.hide-nav {
        transform: translateY(-100%);
    }

    .header__logo {
        width: 150px;
    }

    .header__container {
        display: flex;
        justify-content: space-between;
        align-items: center;
        margin: 0 auto;
        padding-top: 20px;
    }

    .header__nav {
        display: flex;
        justify-content: flex-end;
    }

    .header__nav ul {
        display: flex;
        list-style: none;
        margin: 0;
        padding: 0;
    }

    .header__nav ul ul {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    .header__nav li {
        list-style: none;
        margin: 15px;
        color: white;
    }
}

.nav-link {
    transition: all 0.2s ease-in-out;
    color: #fff;
    text-decoration: none;
    margin: 0 15px;
    padding: 10px;
}

.nav-link:hover {
    font-size: 20px;
    transform: scale(1.1);
}
</style>
