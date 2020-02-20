<template>
    <v-app>
        <app-navigation></app-navigation>
        <v-content transition="slide-x-transition">
            <router-view></router-view>
            <hr>
            <router-link to="/">Home</router-link>
            |
            <router-link to="/about">About</router-link>
        </v-content>
    </v-app>
</template>

<script>
import AppNavigation from '@/components/AppNavigation';

export default {
    name: 'App',
    components: {
        AppNavigation
    }
};
</script>

<style>
</style>