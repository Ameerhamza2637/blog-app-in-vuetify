<template>
    <v-app>
        <Navbar title="Admin Dashboard"/>
    </v-app>
    <Sidebar user="All Users" blog="All Blogs" info="Personal Info"  :useroption="true" adduser="Add User" :blogoption="false"/>
    <Card col="12" wdts="600px"/>
</template>

<script>
    import Sidebar from '@/layouts/Sidebar.vue'
    import Navbar from '@/layouts/Navbar.vue'
    import Card from '@/layouts/Card.vue'
    export default
    {
        components:
        {
            Sidebar,
            Navbar,
            Card
        }
    }
</script>