<template>
    <v-app>
        <v-app-bar
                app
                flat
        >
            <v-spacer></v-spacer>
            <template>
                <p class="text-center font-weight-black ma-0"
                   style="font-family: 'Times New Roman',serif; font-size: 20px">Academy of Magic</p>
                <v-btn-toggle
                        group
                        color="black"
                        borderless>
                    <v-btn text @click="toHome">Home</v-btn>
                    <v-btn text @click="toMembers">Members</v-btn>
                    <v-btn text @click="toPublications">Publications</v-btn>
                    <v-btn text>Gallery</v-btn>
                </v-btn-toggle>
            </template>
            <v-spacer></v-spacer>
            <v-btn text>中文</v-btn>
            <v-spacer></v-spacer>
        </v-app-bar>

        <v-main>
            <v-container fluid>
                <router-view/>
            </v-container>
        </v-main>

        <v-toolbar padless>
            <v-card
                    class="flex"
                    flat
                    tile
            >
                <v-card-text class="black--text text-center">
                    <hr>
                </v-card-text>

                <v-card-text class="py-2 black--text text-center">
                    Copyright © {{ new Date().getFullYear() }} <a href="https://judgementh.github.io/">Judgement.</a>
                    All rights reserved.
                </v-card-text>
            </v-card>
        </v-toolbar>

    </v-app>
</template>

<script>

    export default {
        name: 'App',

        data: () => ({
            //
        }),
        methods: {
            toHome() {
                this.$router.push({path: './'})
            },
            toAbout() {
                this.$router.push({path: './About'})
            },
            toMembers() {
                this.$router.push({path: './members'})
            },
            toPublications(){
                this.$router.push({path:'./publications'})
            }
        }
    };
</script>

<style xml:lang="scss" scoped>
    .v-btn {
        text-transform: none;
    }

    .no-color {
        background-color: unset;
    }
</style>
