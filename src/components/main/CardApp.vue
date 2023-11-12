<template>
    <div class="col-12 col-md-2 mb-5">
        <img :src="thumb" :alt="series" class="mb-3">
        
    </div>
</template>

<script>
export default {
    name: 'CardApp',
    props: {
        thumb: String,
        series: String,
    }
}
</script>

<style lang="scss" scoped>
img {
    width: 100%;
    height: 250px;
    object-fit: cover;
    object-position: top;
}
</style>