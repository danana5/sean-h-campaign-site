<template>
<v-list-item>
    <v-list-item-icon class="pa-0 mr-2">
        <v-btn icon :href="contact.link" target="_blank" class="white--text">
            <v-icon>{{contact.icon}}</v-icon>
        </v-btn>
    </v-list-item-icon>
    <v-list-item-content class="white--text">
        <v-list-item-title>{{contact.value}}</v-list-item-title>
        <v-list-item-subtitle class="white--text">{{contact.name}}</v-list-item-subtitle>
    </v-list-item-content>
</v-list-item>
</template>

<script>
export default {
    name: "ContactList",
    props: {
        contact: {
            type: Object,
            default: function () {
                return {}
            }
        }
    }
}
</script>
