<template>
    <div id="books">
        <section class="hero is-warning is-fullheight">
            <div class="hero-head">
                <div class="container">
                    <h1 class="title">电子书</h1>
                </div>
            </div>
            <div class="hero-body">
                <div class="container">
                    <div class="columns is-desktop">
                        <book v-bind:key="book.id" v-for="book in books"
                              :title="book.title"
                              :image="book.image"
                              :website="book.website"
                              :description="book.description"></book>
                    </div>
                </div>
            </div>

        </section>
    </div>
</template>

<script>
    import data from '@/data/books.json'
    import Book from "../components/Book";

    export default {
        name: "Books",
        components: {Book},
        data: function () {
            return {
                books: data.data
            }
        },
        comments: {
            Book
        }
    }
</script>

<style lang="scss" scoped>
    .hero-head {
        padding: 50px 0px 20px 0px;
    }
</style>