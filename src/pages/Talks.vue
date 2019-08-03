<template>
    <div id="talks">
        <section class="hero is-dark is-fullheight">
            <div class="hero-head">
                <div class="container">
                    <h1 class="title">演讲与分享</h1>
                </div>
            </div>
            <div class="hero-body">
                <div class="container">
                    <div class="columns is-desktop">
                        <Talk v-for="talk in talks" v-bind:key="talk.id" :title="talk.title" :date="talk.date"
                              :link="talk.link" :location="talk.location"></Talk>
                    </div>
                </div>
            </div>

        </section>
    </div>
</template>

<script>
    import Talk from '@/components/Talk'
    import data from '@/data/talks.json'

    export default {
        name: "Talks",
        data: function () {
            return {
                talks: data.data
            };
        },
        components: {
            Talk
        }
    }
</script>

<style lang="scss" scoped>
    .hero-head {
        padding: 50px 0px;
    }
</style>