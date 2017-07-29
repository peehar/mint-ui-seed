<template>
  <div id="app">
    <mt-header :title="title"></mt-header>
    <router-view></router-view>
    <!-- 路由匹配到的组件将渲染在这里 -->
    <mt-tabbar v-model="selected">
      <mt-tab-item id="tab1">
        <img slot="icon" src="./static/home.png"/>
        首页
      </mt-tab-item>
      <mt-tab-item id="tab2">
        发现
      </mt-tab-item>
      <mt-tab-item id="tab3">
        我的
      </mt-tab-item>
    </mt-tabbar>
  </div>
</template>

<script>
import Vue from 'vue'
import { Header, Tabbar, TabItem } from 'mint-ui';

Vue.component(Header.name, Header);
Vue.component(Tabbar.name, Tabbar);
Vue.component(TabItem.name, TabItem);

export default {
    name: 'app',
    data () {
        return {
        msg: 'Welcome to Your Vue.js App',
        title: "fdsafdasf"
        }
    }
}


</script>

<style>

</style>
