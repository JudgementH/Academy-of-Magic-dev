<template>
    <div>
        <v-row
                justify="center">
            <v-col cols="8">
                <v-row
                        justify="center">
                    <v-col align-self="center">
                        <p class="text-h4">About the Lab</p>
                        <p class="text-body-1">
                            <strong>Hogwarts School of Witchcraft and Wizardry</strong>, often shortened to Hogwarts,
                            was
                            the British
                            wizarding school, located in the Scottish Highlands. It accepted magical students from
                            Great Britain and Ireland for enrolment. It was a state-owned school, funded by the
                            Ministry of Magic.
                        </p>
                        <p class="text-body-1">

                            wizarding school, located in the Scottish Highlands. It accepted magical students from
                            Great Britain and Ireland for enrolment. It was a state-owned school, funded by the
                            Ministry of Magic.
                        </p>

                        <p class="text-body-1">
                            wizarding school, located in the Scottish Highlands. It accepted magical students from
                            Great Britain and Ireland for enrolment. It was a state-owned school, funded by the
                            Ministry of Magic.
                        </p>
                    </v-col>
                </v-row>

                <v-row>
                    <v-col cols="4">
                        <div>
                            <v-img src="https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/touhou/youmu.jpg"
                                   max-width="500"></v-img>
                            <p class="text-center subtitle-1 font-weight-bold">fig.1</p>
                        </div>
                    </v-col>

                    <v-col cols="4">
                        <div>
                            <v-img src="https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/touhou/youmu.jpg"
                                   max-width="500"></v-img>
                            <p class="text-center subtitle-1 font-weight-bold">fig.2</p>
                        </div>
                    </v-col>

                    <v-col cols="4">
                        <div>
                            <v-img src="https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/touhou/youmu.jpg"
                                   max-width="500"></v-img>
                            <p class="text-center subtitle-1 font-weight-bold">fig.3</p>
                        </div>
                    </v-col>
                </v-row>

                <v-row
                        justify="center">
                    <v-col>
                        <p class="text-h4">News</p>
                        <ul>
                            <li v-for="item in news" :key="item.id">{{item}}</li>
                        </ul>
                    </v-col>
                </v-row>

            </v-col>
        </v-row>

    </div>
</template>

<script>

    export default {
        name: 'Home',

        components: {},
        data: () => ({
            news: [
                "2021-10-02: Update",
                "2021-09-30: Hello World!",
            ]
        }),
        methods: {}
    }
</script>
