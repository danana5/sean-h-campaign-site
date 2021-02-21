<template>
<v-app>
    <div>
        <v-card dark color="#ffa5ac" flat height="600" tile>
            <v-container fill-height>
                <v-row align="center" justify="center">
                    <v-container>
                        <v-card class="text-center mx-auto" color="indigo darken-4" elevation="12" max-width="450">
                        <v-container>
                            <v-avatar size="200" elevation="12">
                                <v-img src="./assets/profile.png"/>
                            </v-avatar>
                            <h1 class="display-1 font-weight-thin mb-4">Vote Sean Hallahan #1</h1>
                            <h4 class="subheading mb-4">For Clubs and Societies</h4>
                            <div class="body-2">
                                Due to the current circumstances I am unable to meet students on campus and speak to them in person. I have decided 
                                to create this website in an effort to get who I am across to you all, the students. 
                            </div>
                        </v-container>
                    </v-card>
                    </v-container>
                </v-row>
            </v-container>
        </v-card>
        <v-flex id="About">
            <About />
        </v-flex>
        <v-flex id="Contact">
            <Contact />
        </v-flex>
        <Footer />
    </div>

</v-app>
</template>

<script>
import About from "./components/About"
import Contact from "./components/Contact"
import Footer from "./components/Footer"
export default {
    components: {
        About,
        Footer,
        Contact
    },
}
</script>
