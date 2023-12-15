<template lang="">
    <article>
        <div class="container-card-img">
            {{ img }}
        </div>
        <h6 class="series-card">
            {{ serie }}
        </h6>
    </article>
</template>
<script>
export default {
    name: 'CardElement',
    props: [
        'img',
        'serie'
    ]
}
</script>
<style lang="scss">
    article{
        width: 15%;
        height: 220px;
        padding: 1rem;
        margin: .5rem;
        border: 1px solid pink;
    }

    .container-card-img{
        width: 100%;
        height: 70%;
    }

    .series-card{
        color: white;
        text-transform: uppercase;
    }
</style>