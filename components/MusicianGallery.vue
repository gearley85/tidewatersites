<template>
    <div class="brook-gallery-area ptb--150 ptb-md--80 ptb-sm--80 bg_color--1 basic-thine-line">
        <div class="container">
            <div class="row">
                <div class="col-lg-12">
                    <div class="brook-section-title text-center mb--60 mb_md--20 mb_sm--20">
                        <h6 class="heading heading-h6 font-400">GALLERY</h6>
                        <div class="bkseparator--35"></div>
                        <h2 class="heading heading-h2">Newest Images</h2>
                    </div>
                </div>
            </div>
        </div>
        <div class="gallery-wrapper pl--100 pr--100 pl_md--50 pr_md--50 pl_sm--30 pr_sm--30">
            <div class="container-fluid">
                <div class="row">
                    <div class="col-lg-4 mt--30" v-for="(item, index) in images" :key="index">
                        <div class="gallery">
                            <div class="thumb">
                                <img :src="item.thumbnail" alt="image">
                            </div>
                            <div class="hover-overlay">
                                <div class="inner">
                                    <span class="ion ion-android-add"></span>
                                </div>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
    export default {
        data () {
            return {
                images: [
                    {
                        src: "/img/gallery/musician/mmusician-lg-1.jpg",
                        thumbnail: "/img/gallery/musician/mmusician-md-1.jpg"
                    },
                    {
                        src: "/img/gallery/musician/mmusician-lg-2.jpg",
                        thumbnail: "/img/gallery/musician/mmusician-md-2.jpg"
                    },
                    {
                        src: "/img/gallery/musician/mmusician-lg-3.jpg",
                        thumbnail: "/img/gallery/musician/mmusician-md-3.jpg"
                    },
                    {
                        src: "/img/gallery/musician/mmusician-lg-4.jpg",
                        thumbnail: "/img/gallery/musician/mmusician-md-4.jpg"
                    },
                    {
                        src: "/img/gallery/musician/mmusician-lg-5.jpg",
                        thumbnail: "/img/gallery/musician/mmusician-md-5.jpg"
                    },
                    {
                        src: "/img/gallery/musician/mmusician-lg-6.jpg",
                        thumbnail: "/img/gallery/musician/mmusician-md-6.jpg"
                    },
                ]
            }
        },
    };
</script>