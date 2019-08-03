<template>
    <div id="works">
        <section class="hero is-primary is-fullheight">
            <div class="hero-head">
                <div class="container">
                    <h1 class="title">项目</h1>
                </div>
            </div>
            <div class="hero-body">
                <div class="container">
                    <div class="columns is-desktop is-multiline">
                        <Work v-for="work in works" v-bind:key="work.id"
                              :title="work.title"
                              :star="work.star"
                              :link="work.link"
                              :license="work.license"
                              :description="work.description"
                        ></Work>
                    </div>
                </div>
            </div>

        </section>
    </div>
</template>

<script>
    import Work from '@/components/Work'
    import data from '@/data/works.json'

    export default {
        name: "Works",
        data: function () {
            return {
                works: data.data
            }
        },
        components: {
            Work
        }
    }
</script>

<style lang="scss" scoped>
    .hero-head {
        padding: 50px 0px 0px 0px;
    }
</style>