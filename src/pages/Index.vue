<template>
    <Layout>
        <h1>Portfolio</h1>
        <p>
            Lorem ipsum dolor sit amet, consectetur adipisicing elit. Pariatur excepturi labore tempore expedita, et
            iste tenetur suscipit explicabo! Dolores, aperiam non officia eos quod asperiores
        </p>
        <PortfolioItem name="Skagit 60 Website"></PortfolioItem>
    </Layout>
</template>

<script>
    import PortfolioItem from "../components/Portfolio-Item";
    export default {
        components: {PortfolioItem},
        metaInfo: {
            title: 'Home'
        }
    }
</script>

<style>
    .home-links a {
        margin-right: 1rem;
    }
</style>
