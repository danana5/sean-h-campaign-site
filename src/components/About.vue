<template>
<div style="background: #1A237E">
    <v-container class="text-center">
        <h1 class="display-2 font-weight-thin red--text text--lighten-3"> About Me</h1>
        <v-divider dark />
        <v-card flat max-width="900" class="mx-auto" color="transparent">
            <div class="body-1 white--text">Hello! I am Sean, I am a 21 year old lad from Swords in third year Computer Science at Trinity College Dublin.
                I've learned so much and I have gained many unique experiences but I've also been fortunate enough to meet many great people and characters whom I am lucky to
                call friends.<br><br>I am a front-end developer but with a strong interest also with full stack development. I have experience using React.js and Vue.js
                aswell as Python, Java and C.<br><br>Anyways, I played semi-proffesional football for Drogheda United in the League of Ireland. I am obsessed with music and several
                artists such as; Flume, deadmau5,
                Porter Robinson and Brockhampton. Film-wise, I love Christopher Nolan and nearly all of his films, I like Tarantino also and I'm a huge fan of Denis Villeneuve.
            </div>
            <div class="mt-8" width="100">
                <v-carousel cycle interval=5000>
                    <v-carousel-item v-for="(item,i) in items" :key="i" :src="logo(item.src)"></v-carousel-item>
                </v-carousel>
            </div>
        </v-card>
        <v-row class="mt-5">
            <v-img src="../assets/posterA.png" max-height="1000" max-width="600" class="mx-auto"></v-img>
            <v-img src="../assets/posterB.png" max-height="1000" max-width="600" class="mx-auto"></v-img>
        </v-row>
    </v-container>
</div>
</template>

<script>
export default {
    data() {
        return {
            items: [{
                    src: "slidetackle.jpg"
                },
                {
                    src: "team.jpg"
                },
                {
                    src: "footballteam.png"
                },
                {
                    src: "pubpic.png"
                },
                {
                    src: "futsal.jpg"
                },
                {
                    src: "cupwin.png"
                },
            ],
        }
    },
    methods: {
        logo(name) {
            return require("../assets/" + name)
        }
    }
}
</script>
