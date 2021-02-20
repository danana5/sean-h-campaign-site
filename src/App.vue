<template>
<v-app>
    <div>
        <v-card dark color="#ffa5ac" flat height="400" tile>
            <v-container fill-height>
                <v-row align="center" justify="center">
                    <v-card flat class="text-center" color="indigo darken-4">
                        <v-container>
                            <h1 class="display-1 font-weight-thin mb-4">Vote Sean Hallahan #1</h1>
                            <h4 class="subheading mb-4">For Clubs and Societies</h4>
                        </v-container>
                    </v-card>
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
