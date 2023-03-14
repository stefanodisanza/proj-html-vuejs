<template>
    <header class="header">
        <div class="header__container">
            <!-- logo e navbar -->
            <img class="header__logo " src="/images/logotype.png" alt="">
            <nav class="header__nav">
                <ul>
                    <li v-for="link in links" :key="link.id">
                        <a :href="link.url">{{ link.label }}</a>
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
        }
    }

}
</script>

<style lang="scss" scoped>
.header {
    position: fixed;
    top: 0;
    left: 0;
    width: 100%;
    z-index: 1000;
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

    ul {
        display: flex;
        align-items: center;
        justify-content: space-between;
    }

    li {
        list-style: none;
        margin: 15px;
        color: white;
    }
}
</style>```
