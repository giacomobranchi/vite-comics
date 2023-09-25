<script>
import products from '../products'
export default {
    data() {

        return {
            name: 'AppMain',
            products
        }
    }

}
</script>

<template>
    <div class="crop">

    </div>
    <div class="bg_dark">
        <div class="container">
            <span class="current">CURRENT SERIES</span>
            <div class="row">
                <div v-for="product in products" class="col-2">
                    <div class="p-2">
                        <div class="card_header" :style="{ 'background-image': 'url(' + product.thumb + ')' }"
                            style="background-position: top; background-size: cover; background-repeat: no-repeat;">

                        </div>
                        <div class=" text-white py-2">
                            <div class="upper">{{ product.series }}</div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>


<style lang="scss" scoped>
.bg_dark {
    background-color: #1c1c1c;
    position: relative;
    padding: 3rem;
}

.crop {
    height: 450px;

    background-image: url(../assets/img/jumbotron.jpg);
}

.card_header {
    aspect-ratio: 1;
    background-image: url(product.thumb);
}

.current {
    background-color: #0282f9;
    color: white;
    padding: 0.5rem;
    text-align: center;
    margin-top: -2rem;
    display: inline-block;
    font-size: 1.5rem;
    position: absolute;
    top: 0;
    font-weight: bold;
}

img {
    width: 100%;


}

.upper {
    text-transform: uppercase;
}
</style>