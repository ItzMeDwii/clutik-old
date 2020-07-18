<!--
 * Welcome to Clovuer
 * The comments in each files will guide you through your very cool journey
 * discovering what Vue can do.
 -->
<template>
  <div id="app">
    <div id="nav">
      <nav class="py-2 navbar fixed-top navbar-expand-lg">
        <div class="container">
          <a class="navbar-brand font-weight-bold" href="/"><img src="https://cdn.discordapp.com/attachments/521473681566990340/733234555992932403/1594885926650.png" width="64px"></a>
        <button class="navbar-toggler" type="button" data-toggle="collapse" data-target="#navbarSupportedContent"
                aria-controls="navbarSupportedContent" aria-expanded="false" aria-label="Toggle navigation">
          <i class="fas fa-align-justify toggler1"></i>
        </button>
        <div class="collapse navbar-collapse" id="navbarSupportedContent">
          <ul class="navbar-nav mr-auto">
            <li class="nav-item mx-1">
              <a class="nav-link border rounded" v-scroll-to="'#home'" href="#">Home</a>
            </li>
            <li class="nav-item mx-1">
              <a class="nav-link border rounded" v-scroll-to="'#tentang'" href="#">Tentang</a>
            </li>
            <li class="nav-item mx-1">
              <a class="nav-link border rounded" v-scroll-to="'#kegiatan'" href="#">Kegiatan & Fasilitas</a>
            </li>  
            <li class="nav-item mx-1">
              <a class="nav-link border rounded" v-scroll-to="'#tentangweb'" href="#">Tentang Website</a>
            </li>                                   
          </ul>
          <ul class="navbar-nav ml-auto">
            <ThemeChanger/>
          </ul>
        </div>
        </div>
      </nav>
    </div>
    <!--
     * This is where your content will be displayed.
     * Refer to `router/index.ts` for component that will be displayed
     * over a router.
    -->
    <div class="center" id="home">
      <div class="container">
          <img alt="Clutik logo" style="height: 220px; width: 220px" src="https://cdn.discordapp.com/attachments/521473681566990340/733234555992932403/1594885926650.png">
          <h1>Selamat Datang di Club TIK</h1>
          <p>SMA Negeri 2 Kota Mojokerto.</p>
      </div>
    </div>

    <br/>
    <div class="container">
      <hr/>
    </div>
    <br/>

    <div class="center"  id="tentang">
      <div class="container">
        <h1>Tentang CluTik </h1>
        <p>Coming Soon...</p>
      </div>
    </div>

    <br/>
    <div class="container">
      <hr/>
    </div>
    <br/>

    <div class="center" id="kegiatan">
      <div class="container">
        <h1>Kegiatan & Fasilitas</h1>
        <Slideshow/>
      </div>
    </div>

    <br/>
    <div class="container">
      <hr/>
    </div>
    <br/>

    <div class="center" id="tentangweb">
      <div class="container">
        <h1>Tentang Website Ini</h1>
        <p>Coming Soon...</p>
      </div>
    </div>
  </div>
</template>

<!--
 * Clovuer shipped with SCSS/SASS support via node-sass.
-->
<style lang="scss" src="./styles.scss"></style>

<script lang="ts">
  import Vue from "vue"
  import {Component} from "vue-property-decorator"
  import ScrollTo from "vue-scrollto"
  Vue.use(ScrollTo);
  
  /**
   * You can use `@/` as an equivalent for `./src`
   */
  //import LocaleChanger from "@/components/LocaleChanger.vue";
  import ThemeChanger from "@/components/ThemeChanger.vue";
  import Slideshow from "@/components/Slideshow.vue";

  /**
   * @Component decorator is used to declare a Vue Component
   * and including Component into the Vue instance
   */
  @Component({
    name: "App",
    components: {
      ThemeChanger,
      Slideshow
    }
  })
  export default class App extends Vue {
  }
</script>
