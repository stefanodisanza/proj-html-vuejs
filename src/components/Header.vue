<template>
    <header class="main-header">
        <div class="container">
            <img class="logo-header " src="/images/logotype.png" alt="">
            <nav>
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
.main-header {
    text-align: center;
}

.container {
    display: flex;
    align-items: center;
    justify-content: space-between;

}

ul {
    display: flex;
    align-items: center;
    justify-content: space-between;
}

li {
    list-style: none;
    margin: 15px;
}

.logo-header {
    width: 130px;
}
</style>