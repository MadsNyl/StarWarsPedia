<template>
    <header>
        <h1>StarWarsPedia</h1>
        <ul>
            <li v-for="nav in navs" :key="nav"></li>
        </ul>
    </header>
</template>

<script>
export default {
    name: 'Header',
    data(){
        return{
            navs: [
                {
                    href: '/',
                    title: 'persons'
                },
                {
                    href: '/',
                    title: 'planets'
                },
                {
                    href: '/',
                    title: 'films'
                },
                {
                    href: '/',
                    title: 'vehicles'
                },
                {
                    href: '/',
                    title: 'species'
                },
                {
                    href: '/',
                    title: 'starships'
                },
            ]
        }
    }
}
</script>

<style lang="scss">
header {
    width: 100%;
    padding: 10px 0;
    display: flex;
    justify-content: space-between;
    align-items: center;

}
</style>