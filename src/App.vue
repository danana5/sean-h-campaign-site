<template>
    <v-app>
      <div>
            <v-parallax
                dark
                src="./assets/team3.jpg"
            >
                <v-row
                align="center"
                >
                  <v-col class="text-center justify-end">
                      <h1 class="display-1 font-weight-thin mb-4">Vote Sean Hallahan #1</h1>
                      <h4 class="subheading mb-4">For Clubs and Societies</h4>
                  </v-col>
                </v-row>
            </v-parallax>          
        <v-flex id="About">
            <About/>
        </v-flex>
        <v-flex id="Contact">
            <Contact/>
        </v-flex>
        <Footer/>
    </div>

    </v-app>
</template>

<script>
import About from "./components/About"
import Contact from "./components/Contact"
import Footer from "./components/Footer"
export default {
    components:{
        About,
        Footer,
        Contact
    },
}
</script>