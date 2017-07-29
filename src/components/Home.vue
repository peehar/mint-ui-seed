<template>
  <div id="home">
    <h1>Home page</h1>

    <h2>{{msg}}</h2>
    <mt-button type="default">default</mt-button>
    <mt-button type="primary">primary</mt-button>
    <mt-button type="danger">danger</mt-button>
  </div>

</template>

<script>

    import Vue from 'vue'
    import VueRouter from 'vue-router'
    import { Button, Cell } from 'mint-ui'    
    Vue.component(Button.name, Button)
    Vue.component(Cell.name, Cell)

    export default {
    name: 'home',
    data () {
        return {
        msg: 'Welcome to Your Vue.js App'
        }
    }
    }

</script>