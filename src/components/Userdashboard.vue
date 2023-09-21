<template>
    <v-app>
        <Navbar title="User Dashboard"/>
    </v-app>
    <Sidebar blog="All Blogs" info="Personal Info" :useroption="false" addblog="Add Blogs" :blogoption="true"/>
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