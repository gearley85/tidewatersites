<template>
    <div class="service service--1 text-center mt--30">
        <div class="icons">
            <i :class="service.icon"></i>
        </div>
        <div class="content">
            <h4>{{ service.heading }}</h4>
            <p>{{ service.desc }}</p>
            <nuxt-link to="/services-classic" class="service-btn">
                <span>More details</span> 
                <i class="fa fa-arrow-right"></i>
            </nuxt-link>
        </div>
    </div>
</template>

<script>
    export default {
        props: ['service']
    };
</script>