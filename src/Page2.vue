<template>
  <v-ons-page>
    <custom-toolbar :back-label="'Page 1'">Page 2</custom-toolbar>
    <p style="text-align: center">これは2番目のページですよ〜</p>
  </v-ons-page>
</template>

<script>
  import customToolbar from './CustomToolbar';
  import app from './App';

  export default {
    methods: {
      pop() {
        this.pageStack.pop();
      } 
    },
    props: ['pageStack'],
    components: { customToolbar }
  }
</script>
