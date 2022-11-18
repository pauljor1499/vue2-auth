<template>
    <div class="main-content">
        <form @submit="handleSubmit()">
            <v-card width="400">
                <v-card-title> Register </v-card-title>
                <v-card-text>
                    <v-row dense>
                        <v-col cols="12">
                            <v-text-field
                                v-model="first_name"
                                outlined
                                dense
                                solo
                                flat
                                label="First name"
                            />
                            <v-text-field
                                v-model="last_name"
                                outlined
                                dense
                                solo
                                flat
                                label="Last name"
                            />
                            <v-text-field
                                v-model="email"
                                outlined
                                dense
                                solo
                                flat
                                label="E-mail"
                            />
                            <v-text-field
                                v-model="password"
                                outlined
                                dense
                                solo
                                flat
                                label="Password"
                            />
                            <v-btn color="primary" @click="handleSubmit()">
                                CREATE</v-btn
                            >
                        </v-col>
                    </v-row>
                </v-card-text>
            </v-card>
        </form>
    </div>
</template>

<script>
import NavBar from "@/components/NavBar.vue";

export default {
    components: { NavBar },

    data() {
        return {
            first_name: "",
            last_name: "",
            email: "",
            password: "",
        };
    },

    methods: {
        handleSubmit() {
            console.log("submit");
        },
    },
};
</script>

<style scoped>
.main-content {
    padding: 100px;
}

.v-card {
    margin: auto;
}
</style>
