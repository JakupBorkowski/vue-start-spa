<template>
    <navbar
    ></navbar>
    
    <router-view>

    </router-view>
    
</template>

<script>
import Navbar from './components/Navbar.vue';

export default {
    inject: ['$pages'],
    components: {
        Navbar,
    },
    methods: {
        pageCreated(pageObject){
            console.log(pageObject);
            this.$pages.push(pageObject);
        }
    }
}
</script>