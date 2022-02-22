<template>
        <div class="box-series">
        <a :href="thumb">
            <img :src="thumb" :alt="series">
            <p>{{series}}</p>
        </a>    
        </div>
</template>

<script>
export default {
    name: 'CurrentSeries',
    props: {
        "thumb": String,
        "series": String
    },
}
</script>

<style lang="scss" scoped>
    @import "../../assets/style/variables.scss";
    @import "../../assets/style/general.scss";

    
    .box-series {
        margin-right: 2%;
        width: calc(90% / 6);
        height: 7rem;

        &:nth-child(6), &:nth-child(12) {
            margin-right: 0 !important;
        }

        a {
            text-decoration: none;

            &:hover {
                opacity: 0.5;
            }
            
        }

        img {
            width: 100%;
            height: 7rem;
            object-fit: cover;
            object-position: top;

            &:hover {
                transform: scale(1);
            }
        }
        p {
            
            margin: 8% 0;
            width: 100%;
            font-size: 65%;
            text-transform: uppercase;
            color: $headerBackground;
            
        }
    }
</style>