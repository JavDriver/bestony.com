<template>
    <div id="app">
        <Header></Header>
        <Skills></Skills>
        <Works></Works>
        <Books></Books>
        <Talks></Talks>
        <Footer></Footer>

    </div>
</template>

<script>
    import Header from './pages/Header'
    import Works from './pages/Works'
    import Books from './pages/Books'
    import Footer from "./pages/Footer";
    import Talks from './pages/Talks'
    import Skills from "./pages/Skills";

    export default {
        name: 'app',
        components: {
            Footer, Talks, Skills,
            Header, Works, Books
        }
    }
</script>

<style>
    html,
    body,
    #app {
        height: 100%;
    }
</style>
