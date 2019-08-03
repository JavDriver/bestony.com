<template>
    <div id="header">
        <section class="hero is-info is-fullheight">

            <div class="hero-body">
                <div class="container">
                    <div class="columns is-desktop">
                        <div class="column is-12-mobile is-8-desktop">

                            <div class="infobox">
                                <h1 class="title">
                                    你好，我是白宦成 (@bestony)
                                </h1>
                                <h2 class="subtitle">
                                    全栈工程师 & 作者
                                </h2>
                                <h2 class="subtitle social">
                                    <button class="button is-info" @click="emailme">
                                        <b-icon icon="email" size="is-medium"></b-icon>
                                    </button>
                                    <button class="button is-info" @click="twitter">
                                        <b-icon icon="twitter" size="is-medium"></b-icon>
                                    </button>
                                    <button class="button is-info" @click="wordpress">
                                        <b-icon icon="wordpress" size="is-medium" @click="wordpress"></b-icon>
                                    </button>
                                    <button class="button is-info" @click="downloadresume">
                                        <b-icon icon="file" size="is-medium" @click="wordpress"></b-icon>
                                    </button>
                                </h2>
                                <h4 class="has-text-light">
                                    下滑查看更多信息
                                </h4>
                            </div>
                        </div>
                        <div class="column  is-12-mobile is-4-desktop">
                            <img :src="image" alt="HuanCheng Bai" class="avatar">
                        </div>

                    </div>

                </div>
            </div>
        </section>
    </div>
</template>

<script>
    import image from '@/assets/avatar.jpg'

    export default {
        name: "Header",
        data: function () {
            return {
                image
            }
        },
        methods: {
            emailme() {
                window.open("mailto:xiqingongzi@gmail.com")
            },
            twitter() {
                window.open("https://twitter.com/xiqingongzi")
            },
            wordpress() {
                window.open("https://www.ixiqin.com")
            },
            downloadresume() {
                window.open("https://bestony.com/resume.pdf")
            }
        }
    }
</script>

<style lang="scss" scoped>
    .infobox {
        display: flex;
        flex-direction: column;
        justify-content: center;
        align-items: center;
        height: 100%;

        .title {
            margin-bottom: 50px;
        }

        .subtitle {
            margin-bottom: 50px;

            .social {
                display: flex;
                flex-direction: row;
                width: 100%;
                justify-content: space-between;
            }
        }
    }
</style>