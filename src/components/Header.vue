<template>
    <header class="header">
        <strong>
            <g-link to="/" class="title">Raymond DeVries</g-link>
        </strong>
        <nav class="nav">
            <g-link class="nav__link" to="/">Home</g-link>
            <g-link class="nav__link" to="/about-me/">About Me</g-link>
        </nav>
    </header>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>
    .header {
        text-align: center;
        display: flex;
        justify-content: space-evenly;
        flex-wrap: wrap;
        align-items: center;
    }

    .header:visited {
        text-decoration: none;
    }

    .nav__link {
        margin-left: 20px;
        text-decoration: none;
    }

    .nav__link:visited, .nav__link:link {
        text-decoration: none;
        color: white;
    }

    .title {
        color: #e58032;
        text-decoration: none;
        font-size: 50px;

    }
</style>