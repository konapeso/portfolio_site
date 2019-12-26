<template>
    <v-row

      justify="center"
    >


    <v-tool-bar app height="90px" :elevate-on-scroll="elevateOnScroll">
        <v-toolbar-title>Page title</v-toolbar-title>
    </v-tool-bar>
    

    </v-row>
 

    
</template> 

<script>
export default{
    data() {
        return {
            elevateOnScroll: false,

        }
    }
};

</script>