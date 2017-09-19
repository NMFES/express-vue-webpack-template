<template>
    <div>App</div>
</template>
<script type="text/javascript">
    import 'bootstrap';
    import axios from 'axios';

    export default {
        data() {
            return {

            }
        },
        components: {},
        created() {
            var socket = io('http://localhost:3000');
        },
        mounted() {

        },
        watch: {

        },
        methods: {

        }
    }
</script>
<style lang="scss">
    $fa-font-path: "~font-awesome/fonts";
    @import "~font-awesome/scss/font-awesome";

    @import "~bootstrap/scss/bootstrap";
    @import "../sass/styles";
</style>