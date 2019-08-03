<template>
    <div class="talk column is-one-quarter-desktop is-half-mobile">
        <div class="card">
            <header class="card-header">
                <p class="card-header-title">
                    {{title}}
                </p>
            </header>
            <div class="card-content">
                <div class="content">
                    {{description}}
                </div>
            </div>
            <footer class="card-footer">
                <div class="card-footer-item">
                    <b-icon
                            icon="star"
                            size="is-small">
                    </b-icon>
                    {{star}}
                </div>
                <div class="card-footer-item">
                    {{license}}
                </div>
                <a target="_blank" :href="link" class="card-footer-item">Github</a>
            </footer>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Work",
        props: {
            title: String,
            link: String,
            star: String,
            license: String,
            description: String
        }
    }
</script>

<style scoped>

</style>