<template>
    <v-app>
        <v-main>
            <NavBar />
            <router-view />
        </v-main>
    </v-app>
</template>

<script>
import NavBar from "@/components/NavBar.vue";

export default {
    components: { NavBar },
};
</script>

<style>
* {
    text-decoration: none;
    text-transform: none;
}
</style>
