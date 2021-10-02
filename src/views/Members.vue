<template>
    <div>
        <v-row justify="center">
            <v-col cols="8">
                <div class="pb-10" v-if="professor.length > 0">
                    <p class="text-h4">Professors</p>
                    <v-row>
                        <v-col cols="2"
                               v-for="(item,i) in professor"
                               :key="i">
                            <div class="text-center">
                                <v-img :src="item.avatar" class="rounded-circle" min-width="130"
                                       max-width="130"></v-img>
                                <div class="font-weight-bold">{{item.name}}</div>
                                <div>
                                    <a :href="item.website" v-if="item.website">[web]</a>
                                    <a :href="item.github" v-if="item.github">[github]</a>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </div>

                <div class="pb-10" v-if="phd.length > 0">
                    <p class="text-h4">PhD Students</p>
                    <v-row>
                        <v-col cols="2"
                               v-for="(item,i) in phd"
                               :key="i">
                            <div class="text-center">
                                <v-img :src="item.avatar" class="rounded-circle" min-width="130"
                                       max-width="130"></v-img>
                                <div class="font-weight-bold">{{item.name}}</div>
                                <div>
                                    <a :href="item.website" v-if="item.website">[web]</a>
                                    <a :href="item.github" v-if="item.github">[github]</a>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </div>

                <div class="pb-10" v-if="master.length > 0">
                    <p class="text-h4">Master Students</p>
                    <v-row>
                        <v-col cols="2"
                               v-for="(item,i) in master"
                               :key="i">
                            <div class="text-center">
                                <v-img :src="item.avatar" class="rounded-circle" min-width="130"
                                       max-width="130"></v-img>
                                <div class="font-weight-bold">{{item.name}}</div>
                                <div>
                                    <a :href="item.website" v-if="item.website">[web]</a>
                                    <a :href="item.github" v-if="item.github">[github]</a>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </div>

                <div class="pb-10" v-if="undergraduate.length > 0">
                    <p class="text-h4">Undergraduate Students</p>
                    <v-row>
                        <v-col cols="2"
                               v-for="(item,i) in undergraduate"
                               :key="i">
                            <div class="text-center">
                                <v-img :src="item.avatar" class="rounded-circle" min-width="130"
                                       max-width="130"></v-img>
                                <div class="font-weight-bold">{{item.name}}</div>
                                <div>
                                    <a :href="item.website" v-if="item.website">[web]</a>
                                    <a :href="item.github" v-if="item.github">[github]</a>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </div>

                <div class="pb-10" v-if="alumni.length > 0">
                    <p class="text-h4">Alumni</p>
                    <v-row>
                        <v-col cols="2"
                               v-for="(item,i) in alumni"
                               :key="i">
                            <div class="text-center">
                                <v-img :src="item.avatar" class="rounded-circle" min-width="130"
                                       max-width="130"></v-img>
                                <div class="font-weight-bold">{{item.name}}</div>
                                <div>
                                    <a :href="item.website" v-if="item.website">[web]</a>
                                    <a :href="item.github" v-if="item.github">[github]</a>
                                </div>
                            </div>
                        </v-col>
                    </v-row>
                </div>

            </v-col>
        </v-row>
    </div>
</template>

<script>
    export default {
        name: "Members",
        data: () => ({
            professor: [{
                avatar: 'https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/avatar/akari.jpeg',
                name: 'Akari',
                website: 'https://www.baidu.com',
                github: 'https://www.github.com'
            }, {
                avatar: 'https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/avatar/akari.jpeg',
                name: 'Akari',
                website: 'https://www.baidu.com',
                github: 'https://www.github.com'
            }, {
                avatar: 'https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/avatar/akari.jpeg',
                name: 'Akari',
                website: 'https://www.baidu.com',
                github: 'https://www.github.com'
            }],
            phd: [],
            master: [],
            undergraduate: [],
            alumni: [],
        }),
    }
</script>

<style scoped>

</style>