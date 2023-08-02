<template>
    <div class="main-container">
        <HeaderForOffCanvasBlack @toggleFullpageMenu="fullpageOpen = !fullpageOpen" @togglenav="navOpen = !navOpen" @toggleSearch="searchOpen = !searchOpen" />

        <OffcanvasMenu :class="{'is-visiable' : fullpageOpen}" @toggleFullpageMenu="fullpageOpen = !fullpageOpen" />
        <OffCanvasMobileMenu :class="{'show-mobile-menu' : navOpen}" @togglenav="navOpen = !navOpen" />
        <SearchPopup :class="{'search-popup-open' : searchOpen}" @toggleSearch="searchOpen = !searchOpen" />

        <div class="presentation-home">
            <swiper
                :speed="1000"
                :loop="false"
                :mousewheel="true"
                :direction="'vertical'"
                :pagination="swiperOptions.pagination"
            >
                <swiper-slide class="bg-image-1 bg-cover">
                    <div class="presentation-slider-wrapper">
                        <div class="presentation-inner">
                            <div class="inner slider">
                                <h2 class="heading text-white">tidewater <br> sites</h2>
                            </div>
                        </div>
                    </div>
                </swiper-slide>

                <swiper-slide>
                    <div class="presentation-slider-wrapper">
                        <div class="presentation-inner">
                            <div class="inner about-inner">
                                <div class="row">
                                    <div class="col-md-6">
                                        <div class="content">
                                            <h6 class="heading heading-h6 theme-color">PHILOSOPHY</h6>
                                            <div class="title mt--40 mb--50">
                                                <h2 class="heading heading-h2">Tidewater Sites wants to help your small business grow!</h2>
                                            </div>
                                            <p class="bk_pra">We are ready to create your first website, or bring your existing site up to date. We believe in clean & mobile-friendly designs.</p>
                                        </div>
                                    </div>
                                    <div class="col-md-6 d-none d-md-block">
                                        <div class="thumbnail video-with-thumb">
                                            <img src="/img/slider/presentation/home-presentation-image-03.png" alt="multi-purpose">
                                            <!-- Start Single Popup -->
                                            <!-- <div class="video-btn position--center">
                                                <a class="play__btn" href="https://www.youtube.com/watch?v=9No-FiEInLA" target="_blank">
                                                    <div class="video-icon third-icon"></div>
                                                </a>
                                            </div> -->
                                            <!-- End Single Popup -->
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </swiper-slide>

                <swiper-slide class="bg-image-2 bg-cover">
                    <div class="presentation-slider-wrapper">
                        <div class="presentation-inner">
                            <div class="inner about-service">
                                <div class="container">
                                    <div class="row">
                                        <div class="col-lg-4 col-md-4 d-none d-md-block">
                                            <div class="thumb">
                                                <img src="/img/slider/presentation/iphone-02.png" alt="Multipurpose">
                                            </div>
                                        </div>
                                        <div class="col-lg-8 col-md-8">
                                            <div class="row">
                                                <div class="col-lg-12">
                                                    <div class="brook-section-title text-start">
                                                        <h2 class="heading heading-h2 second-font text-white">Why we're different</h2>
                                                    </div>
                                                </div>

                                                <!-- Start Single Service -->
                                                <div class="col-lg-6 d-none d-md-block mt--50">
                                                    <div class="single-motive-speach">
                                                        <div class="icon">
                                                            <i class="ion-pricetag theme-color"></i>
                                                        </div>
                                                        <div class="content text-start">
                                                            <h4 class="text-white">Up front pricing</h4>
                                                            <p class="bk_pra heading-font text-white">We know every penny counts in your small business!</p>
                                                        </div>
                                                    </div>
                                                </div>
                                                <!-- End Single Service -->

                                                <!-- Start Single Service -->
                                                <div class="col-lg-6 d-none d-md-block mt--50">
                                                    <div class="single-motive-speach">
                                                        <div class="icon">
                                                            <i class="ion-ios-time theme-color"></i>
                                                        </div>
                                                        <div class="content text-start">
                                                            <h4 class="text-white">No guesswork</h4>
                                                            <p class="bk_pra heading-font text-white">We know you don't have time to scroll through pages of templates, that's why we only offer 2 to make things simple.</p>
                                                        </div>
                                                    </div>
                                                </div>
                                                <!-- End Single Service -->

                                                <!-- Start Single Service -->
                                                <div class="col-lg-6 mt--50">
                                                    <div class="single-motive-speach">
                                                        <div class="icon">
                                                            <i class="ion-calendar theme-color"></i>
                                                        </div>
                                                        <div class="content text-start">
                                                            <h4 class="text-white">Monthly Updates</h4>
                                                            <p class="bk_pra heading-font text-white">Let us help update your site! Weekly or monthly specials? No problem, for a small monthly fee we will keep your content up to date.</p>
                                                        </div>
                                                    </div>
                                                </div>
                                                <!-- End Single Service -->

                                                <!-- Start Single Service -->
                                                <div class="col-lg-6 mt--50">
                                                    <div class="single-motive-speach">
                                                        <div class="icon">
                                                            <i class="ion-locked theme-color"></i>
                                                        </div>
                                                        <div class="content text-start">
                                                            <h4 class="text-white">Security</h4>
                                                            <p class="bk_pra heading-font text-white">We will help make sure you security certificate is up to date so your customers feel safe.</p>
                                                        </div>
                                                    </div>
                                                </div>
                                                <!-- End Single Service -->

                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </swiper-slide>

                <swiper-slide>
                    <div class="presentation-slider-wrapper">
                        <div class="presentation-inner">
                            <div class="inner skill-area">
                                <div class="container">
                                    <div class="row">
                                        <div class="col-lg-9 col-md-12">
                                            <div class="row">
                                                <div class="col-lg-12">
                                                    <div class="skill-content">
                                                        <h2 class="heading heading-h2 theme-color">Here to meet your small business needs!</h2>
                                                    </div>
                                                </div>
                                                <!-- <div class="col-xl-2 d-none d-xl-block">
                                                    <div class="what-do mt--70 mt_lg--30 mt_md--30 mt_sm--20">
                                                        <div class="basic-separator line-3"></div>
                                                    </div>
                                                </div> -->
                                                <div class="col-xl-4 col-lg-6 col-md-6 col-sm-12 d-none d-md-block">
                                                    <div class="what-do mt--70 mt_lg--30 mt_md--30 mt_sm--20">
                                                        <div class="content">
                                                            <h5 class="heading heading-h5">Low Cost</h5>
                                                            <div class="bkseparator--20"></div>
                                                            <p class="bk_pra">For $1,500* we will deliver you a mobile friendly, fresh design ready to serve your customers</p>
                                                            <p><i>$800 up front, non-refundable payment</i></p>
                                                        </div>
                                                        <div class="content">
                                                            <h5 class="heading heading-h5">SEO</h5>
                                                            <div class="bkseparator--20"></div>
                                                            <p class="bk_pra">Let us help you with your SEO strategy and get your site on the top search engines and in front of your customers.</p>
                                                        </div>
                                                    </div>
                                                </div>
                                     
                                                <div class="col-xl-4 col-lg-6 col-md-6 col-sm-12 offset-xl-1">
                                                    <div class="what-do mt--70 mt_lg--30 mt_md--30 mt_sm--20">
                                                        <div class="content">
                                                            <h5 class="heading heading-h5">Limited template options to save you time</h5>
                                                            <div class="bkseparator--20"></div>
                                                            <p class="bk_pra">Running a small business is time consuming. You don't want to have to scroll through pages and pages of templates. 
                                                                Pick one of our two ready made templates and get back to running your small business.</p>
                                                        </div>
                                                    </div>
                                                </div>
                                              
                                            </div>
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </swiper-slide>

                <swiper-slide class="bg-image-3 bg-cover">
                    <div class="presentation-slider-wrapper">
                        <div class="presentation-inner contact-address-wrapper">
                            <div class="inner">
                                <div class="container">
                                    <div class="row">
                                        <div class="col-lg-7 col-md-12 col-12">
                                            <div class="row">
                                                <div class="col-lg-12">
                                                    <div class="brook-section-title mb--55 mb_sm--30 mb_md--30">
                                                        <h3 class="heading heading-h3 text-white">Contact us to learn more.</h3>
                                                    </div>
                                                </div>
                                                <div class="col-lg-6 col-md-6 col-12">


                                                    <div class="classic-address text-start mt--60 mt_sm--30 mt_md--30">
                                                        <h4 class="heading heading-h4 text-white text-white">Message us</h4>
                                                        <div class="desc mt--15">
                                                            <p class="bk_pra line-height-2-22 text-white">gavin@tidewatersites.com <br></p>
                                                        </div>
                                                    </div>
                                                </div>
                                                <div class="col-lg-6 col-md-6 col-12 mt_sm--30 d-none d-md-block">
                                                    <div class="footer-widget text-var--2 menu--about">
                                                        <h2 class="widgettitle text-white">About us</h2>
                                                        <div class="footer-menu">
                                                            <ul class="ft-menu-list bk-hover">
                                                                <li><a href="#">About Us</a></li>

                                                                <li><a href="#">Contact</a></li>
                                                            </ul>
                                                        </div>
                                                    </div>
                                                </div>
                                            </div>
                                        </div>
                                        <div class="col-lg-5 col-md-6 d-none d-lg-block">
                                            <!-- <div class="google-map-area bg_color--1 text-center">
                                                <div class="brook-section-title">
                                                    <h3 class="heading heading-h3">Default Style</h3>
                                                </div>
                                                <iframe class="contact-map" src="https://www.google.com/maps/embed?pb=!1m18!1m12!1m3!1d2136.986005919501!2d-73.9685579655238!3d40.75862446708152!2m3!1f0!2f0!3f0!3m2!1i1024!2i768!4f13.1!3m3!1m2!1s0x89c258e4a1c884e5%3A0x24fe1071086b36d5!2sThe%20Atrium!5e0!3m2!1sen!2sbd!4v1585132512970!5m2!1sen!2sbd" allowfullscreen="" aria-hidden="false" tabindex="0"></iframe>
                                            </div> -->
                                        </div>
                                    </div>
                                </div>
                            </div>
                        </div>
                    </div>
                </swiper-slide>
            </swiper>

            <!-- Add Pagination -->
            <div class="swiper-pagination"></div>
        </div>
    </div>
</template>

<script>
    import { Swiper, SwiperSlide } from "swiper/vue"
    import SwiperCore, { Pagination, Mousewheel } from 'swiper/core'
    SwiperCore.use([Pagination, Mousewheel])

    import "swiper/css/mousewheel"
    export default {
        components: {
            Swiper,
            SwiperSlide,
            HeaderForOffCanvasBlack: () => import('@/components/HeaderForOffCanvasBlack'),
            OffcanvasMenu: () => import('@/components/OffcanvasMenu'),
            OffCanvasMobileMenu: () => import('@/components/OffCanvasMobileMenu'),
            SearchPopup: () => import('@/components/SearchPopup'),
        },

        data() {
            return {
                navOpen: false,
                searchOpen: false,
                fullpageOpen: false,
                
                swiperOptions: {
                    pagination: {
                        el: '.swiper-pagination',
                        clickable: true,
                    },
                },
            }
        }
    };
</script>

<style lang="scss">
    .presentation-home {
        .swiper-wrapper {
            max-height: 100vh;
        }
    }

    .vue-map-container {
        height: 500px;
        // res
        @media #{$sm-layout}{
            height: 350px;
        }
    }
</style>