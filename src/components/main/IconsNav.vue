<template>
    <div class="merchandiseIcon">
        <div class="text-uppercase container">
            <ul class="nav d-flex align-items-center justify-content-between ">
                <li class="nav-item" v-for="(link, index) in iconsnav" :key="index">
                    <div class="d-flex align-items-center">
                        <img :src="link.imageIcon">
                        <a class="nav-link" :href="link.url">{{ link.text }}</a>

                    </div>

                </li>
            </ul>
        </div>

    </div>
</template>

<script>
export default {
    name: 'IconsNav',
    data() {
        return {
            iconsnav: [
                {
                    text: 'Digital Comics',
                    imageIcon: '/images/buy-comics-digital-comics.png',
                    url: '#',
                },
                {
                    text: 'DC Merchandise',
                    imageIcon: '/images/buy-comics-merchandise.png',
                    url: '#',
                },
                {
                    text: 'Subscription',
                    imageIcon: '/images/buy-comics-subscriptions.png',
                    url: '#',
                },
                {
                    text: 'Comic Shop Locator',
                    imageIcon: '/images/buy-comics-shop-locator.png',
                    url: '#',
                },
                {
                    text: 'Dc Power Visa',
                    imageIcon: '/images/buy-dc-power-visa.svg',
                    url: '#',
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
.merchandiseIcon {
    background-color: #0282f9;
    padding: 35px;
    margin: 0 auto;
}

a {
    color: white;
}

img {
    width: 45px;
    height: 45%;
}
</style>