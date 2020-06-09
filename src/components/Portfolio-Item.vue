<template>
    <div class="container">
        <div class="item">
            <h1>{{name}}</h1>
        </div>
        <div class="overlay">
            <h1>Deployment</h1>
            <h1>Source Code</h1>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Portfolio-Item",
        props: ['name']
    }
</script>

<style scoped>
    .container {
        --item-height: 300px;

        position: relative;
        min-height: var(--item-height);
    }

    .item {
        height: var(--item-height);
        background: rgb(20, 86, 87);
        background: linear-gradient(30deg, rgb(20, 86, 87) 0%, rgb(7, 62, 99) 100%);
        border-radius: 15px;
        text-align: center;
        opacity: 1;
        display: block;
        width: 100%;
        transition: .5s ease;
        backface-visibility: hidden;
    }

    .overlay {
        display: flex;
        flex-wrap: wrap;
        justify-content: space-between;
        transition: .5s ease;
        opacity: 0;
        position: absolute;
        top: 50%;
        left: 50%;
        transform: translate(-50%, -50%);
        text-align: center;
        width: 65%;
        margin: 0 auto;
    }

    .container:hover .item {
        opacity: 0.5;
    }

    .container:hover .overlay {
        opacity: 1;
    }

    .item h1 {
        padding: 30px;
        /*noinspection CssInvalidFunction*/
        font-size: min(6.5vw, 80px);
    }

    .overlay h1 {
        padding: 10px;
        margin: 20px auto;
        /*noinspection CssInvalidFunction*/
        font-size: min(6.5vw, 50px);
    }


</style>