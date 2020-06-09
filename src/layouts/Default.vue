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
        font-family: 'Comfortaa', sans-serif;
        line-height: 1.5;
        background: #1F1F1F;
        color: white;
    }

    .layout {
        padding: 10px 50px;
        max-width: 1000px;
        margin: 0 auto;
    }


</style>
