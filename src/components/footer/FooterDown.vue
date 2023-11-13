<template>
    <section class="d-flex footerdo">
        <div class="container d-flex justify-content-between align-items-center ">
            <button class="btn text-uppercase">Sign-up Now!</button>
            <ul class="nav align-items-center">
                <li>Follow Us</li>
                <li v-for="(social, index) in iconsfooter" class="icons" :key="index">
                    <img :src="social.image">
                </li>
            </ul>
        </div>

    </section>
</template>

<script>
export default {
    name: 'FooterDown',
    data() {
        return {
            iconsfooter: [
                {
                    image: '/images/footer-facebook.png'
                },
                {
                    image: '/images/footer-twitter.png'
                },
                {
                    image: '/images/footer-youtube.png'
                },
                {
                    image: '/images/footer-pinterest.png'
                },
                {
                    image: '/images/footer-periscope.png'
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>

.footerdo{
    background-color:rgb(48, 48, 48) ;
    padding: 20px;
}
    .btn {
        color: white;
        font-size: 20px;
        border: 2px solid #0282f9;
        margin-left: 20px;
    }
    .icons{
        margin: 5px;
    }


ul {
    list-style: none;
    font-size: 20px;
    color: white;
    margin-right: 20px;

    .text-uppercase {
        color: #0282f9
    }
}
</style>