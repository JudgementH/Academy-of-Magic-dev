<template>
    <div>
        <v-row justify="center">
            <v-col cols="8">
                <div>
                    <p class="text-h4">Publications</p>
                    <p class="subtitle-1"><em>'*' indicates corresponding author.</em></p>

                    <v-row v-for="(item,i) in papers" :key="i">
                        <v-col cols="3" v-if="item.image">
                            <v-img :src="item.image" alt="" max-width="300px"></v-img>
                        </v-col>
                        <v-col cols="9">
                            <p class="text-h5 font-weight-bold ma-0">{{item.title}}</p>
                            <p class="subtitle-1 ma-0">{{item.authors}}</p>
                            <p class="subtitle-2 ma-0">{{item.platform}}</p>
                            <p class="body-1">
                                <a :href="item.page" v-if="item.page">[page]</a>
                                <a :href="item.paper" v-if="item.paper">[paper]</a>
                                <a :href="item.supplementary" v-if="item.supplementary">[supplementary]</a>
                                <a :href="item.code" v-if="item.code">[code]</a>
                            </p>
                        </v-col>
                    </v-row>

                </div>
            </v-col>
        </v-row>
    </div>
</template>

<script>
    export default {
        name: "Publications",
        data: () => ({
            papers: [{
                image: 'https://cdn.jsdelivr.net/gh/JudgementH/image-host/anime/touhou/youmu.jpg',
                title: "fox say this is paper's title.",
                authors: "Author1#,author2#,author3*",
                platform: "xxx Conference",
                page: "https://www.baidu.com",
                paper: "https://www.baidu.com",
                supplementary: "https://www.baidu.com",
                code: "github.com"
            }, {
                title: "fox2 say this is paper's title.",
                authors: "Author1#,author2#,author3*",
                platform: "xxx Conference",
                page: "https://www.baidu.com",
                code: "github.com"
            }]
        }),
    }
</script>

<style scoped>

</style>