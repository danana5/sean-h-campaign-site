<template>
<div style="background: #1A237E">
    <v-container class="text-center">
        <h1 class="display-2 font-weight-thin red--text text--lighten-3">Who I am and Why am I Running?</h1>
        <v-divider dark />
        <v-card flat max-width="900" class="mx-auto mt-3" color="red lighten-3">
            <div class="body-1 white--text pa-4">Hey my name is Sean Hallahan, I am 20 years old and I am in my third year of
                Computing in NCI. Like most, when I started college I knew very little people but now I have made friends
                and memories for life. I want to give back to this college and the students that have made my experience
                so great. I hope to achieve this through the role of Clubs and Societies officer.<br><br>I feel suited to this role as my contributions so far in NCI relates positively
                to the commitments found in the role of C&S officer.
                I put myself forward for Class Rep in my first year of Computing and now, three years later I have continued to be voted in by my course to represent them by being a
                voice for my peers.
                Throughout the three years I have grown as a leader for my classmates and gained the confidence and ability to problem solve and be heard by those who run our college.
                The connection I’ve
                made with my peers by being someone they can come to with any questions or queries or even just for a chat has been such an invaluable experience for me, and I want to
                continue this.<br><br>I understand from my own personal experience how important it is to be involved in an environment that makes you feel valued and appreciated. For me,
                this was NCI football. I nervously trialed for the team in my first year and to my surprise was accepted with open arms. From there, I stuck with the team to now be a part
                of the committee and currently in the role of Social Media Manager. Although my experience was great, I know for a lot of people putting
                yourself out there can be very difficult which is why, if elected, I will ensure that all C&S’s are welcoming to new members just like I was.<br><br> But let’s get back to who
                I am for a second. I love my family and friends, having a laugh, good food and drink, travelling, and meeting new people. I am honest and I will ensure that any issue you bring to
                me, no matter how small, will be given my 100% attention and commitment to resolve in a fair and supportive manner.<br><br>Thank you for reading, please feel free to read through
                my manifesto
                and to contact me on any of the outlets bellow with any concerns or queries.<br><br>#VoteH
            </div>
        </v-card>
        <v-card max-width="1100" color="transparent" flat tile class="mx-auto mt-3">
            <v-carousel cycle interval=5000 height="600">
                <v-carousel-item v-for="(item,i) in items" :key="i" :src="logo(item.src)"></v-carousel-item>
            </v-carousel>
        </v-card>
        <v-row class="mt-5">
            <v-container>
                <v-img src="../assets/posterA.png" max-height="1000" max-width="600" class="mx-auto" position="center center"></v-img>
                <v-img src="../assets/posterB.png" max-height="1000" max-width="600" class="mx-auto mt-5" position="center center"></v-img>
            </v-container>
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
                    src: "pubcrawl.png"
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
