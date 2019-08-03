<template>
    <div class="book column is-one-quarter-desktop is-half-mobile">
        <div class="card">
            <div class="card-image">
                <figure class="image is-16by9">
                    <img :src="image" :alt="title">
                </figure>
            </div>

            <div class="card-content">
                <div class="media">
                    <div class="media-content">
                        <p class="title is-4">{{title}}</p>
                    </div>
                </div>
                <div class="content">
                    {{description}}
                </div>
            </div>
            <footer class="card-footer">
                <a target="_blank" :href="website" class="card-footer-item">查看电子书</a>
            </footer>
        </div>

    </div>
</template>

<script>
    export default {
        name: "Book",
        props: {
            title: String,
            image: String,
            description: String,
            website: String,
        }
    }
</script>

<style scoped>

</style>