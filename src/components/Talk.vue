<template>
    <div class="talk column is-one-quarter-desktop is-half-mobile">
        <div class="card">

            <div class="card-content">
                <div class="media">
                    <div class="media-content">
                        <p class="title is-4 has-text-black">{{title}}</p>
                    </div>
                </div>
                <div class="content">
                    {{location}}
                    <br>
                    <time :datetime="date">{{date}}</time>
                </div>
            </div>
            <footer class="card-footer">
                <a target="_blank" :href="link" class="card-footer-item">查看演讲详情</a>
            </footer>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Talk",
        props: {
            title: String,
            link: String,
            date: String,
            location: String,
        }
    }
</script>

<style scoped>

</style>