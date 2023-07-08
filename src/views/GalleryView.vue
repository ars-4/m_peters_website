<template>
    <div class="gallery">
        <div class="row">
            <div class="col-md-2">
                <AdBox />
                <AdBox class="pc-only" />
            </div>
            <div class="col-md-8">
                <br>
                <h1 class="text-center">Gallery</h1>
                <hr>
                <div class="images row">
                    <div class="col-4" v-for="image in images">
                        <ImageBox />
                    </div>
                </div>
            </div>
            <div class="col-md-2">
                <AdBox />
                <AdBox />
            </div>
        </div>
    </div>
</template>

<style>

.gallery .images .col-4 {
    margin-bottom: 25px;
}

</style>

<script>

import { defineComponent } from 'vue';
import ImageBox from '@/components/ImageBoxComponent.vue';
import AdBox from '@/components/AdComponent.vue';

export default defineComponent({
    components: {
        ImageBox,
        AdBox
    },
    data(){return{
        images: [
            'One', 'Two', 'Three',
            'One', 'Two', 'Three'
        ]
    }}
})

</script>