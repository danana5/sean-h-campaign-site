<template>
<div style="background: #1A237E">
    <v-container>
        <div class="text-center">
            <h1 class="display-2 font-weight-thin red--text text--lighten-3">Contact Me</h1>
        </div>
        <v-divider dark />
        <v-layout wrap>
            <v-flex wrap v-for="(contact, i) in contactLinks" :key="i">
                <ContactList :contact="contact" />
            </v-flex>
        </v-layout>
    </v-container>
</div>
</template>

<script>
import ContactList from "./ContactList"
export default {
    components: {
        ContactList
    },
    data() {
        return {
            contactLinks: [{
                    name: "Email",
                    value: "x18392221@student.ncirl.ie",
                    link: "mailto:x18392221@student.ncirl.ie",
                    icon: "mdi-email"
                },
                {
                    name: "LinkedIn",
                    value: "Sean Hallahan",
                    link: "https://www.linkedin.com/in/sean-hallahan-sh20/",
                    icon: "mdi-linkedin"
                },
                {
                    name: "Snapchat",
                    value: "halooooooo",
                    link: "https://www.snapchat.com/l/en-gb/",
                    icon: "mdi-snapchat"
                },
                {
                    name: "Facebook",
                    value: "Sean Hallahan",
                    link: "https://www.facebook.com/sean.hallahan.58",
                    icon: "mdi-facebook"
                },
                {
                    name: "Instagram",
                    value: "seanh_cs",
                    link: "https://www.instagram.com/seanh_cs/",
                    icon: "mdi-instagram"
                }
            ]
        }
    }
}
</script>
