<template>
    <div class="layout">
    <Header/>
        <slot/>
    </div>
</template>

<static-query>
    query {
    metadata {
    siteName
    }
    }
</static-query>

<script>
    import Header from "../components/Header";

    export default {
        components: {
            Header
        }
    }
</script>

<style>
    @import url('https://fonts.googleapis.com/css2?family=Comfortaa&display=swap');

    body {
        font-family: 'Comfortaa', cursive;
        margin: 50px 10px;
        padding: 0;
        line-height: 1.5;
        background: #1F1F1F;
        color: white;
    }

    .layout {
        max-width: 760px;
        margin: 0 auto;
        padding-left: 20px;
        padding-right: 20px;
    }
</style>
