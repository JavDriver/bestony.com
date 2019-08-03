<template>
    <div id="skills">
        <section class="hero is-success is-fullheight">
            <div class="hero-head">
                <div class="container">
                    <h1 class="title">技能</h1>
                </div>
            </div>
            <div class="hero-body">
                <div class="container">
                    <div class="columns is-desktop">
                        <div class="column is-full-mobile">
                            <div class="skills-box">
                                <h2 class="subtitle">小程序</h2>
                                <b-progress size="is-medium" :value="95" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">PHP</h2>
                                <b-progress size="is-medium" :value="80" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">Laravel</h2>
                                <b-progress size="is-medium" :value="80" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">Node.js</h2>
                                <b-progress size="is-medium" :value="80" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">Egg.js</h2>
                                <b-progress size="is-medium" :value="70" type="is-info" show-value
                                            format="percent"></b-progress>
                            </div>
                        </div>
                        <div class="column is-full-mobile">
                            <div class="skills-box">
                                <h2 class="subtitle">Vue.js</h2>
                                <b-progress size="is-medium" :value="80" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">React.js</h2>
                                <b-progress size="is-medium" :value="75" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">阿里云</h2>
                                <b-progress size="is-medium" :value="90" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">腾讯云</h2>
                                <b-progress size="is-medium" :value="90" type="is-info" show-value
                                            format="percent"></b-progress>
                                <h2 class="subtitle">Git</h2>
                                <b-progress size="is-medium" :value="80" type="is-info" show-value
                                            format="percent"></b-progress>
                            </div>
                        </div>

                    </div>

                </div>
            </div>

        </section>
    </div>
</template>

<script>
    export default {
        name: "Skills"
    }
</script>

<style lang="scss" scoped>
    .hero-head {
        padding-top: 50px;
    }

    .skills-box {
        display: flex;
        flex-direction: column;
        justify-content: flex-start;
        align-content: flex-start;
    }
</style>