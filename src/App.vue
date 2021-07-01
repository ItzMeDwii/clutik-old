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
              <a class="nav-link border rounded" v-scroll-to="'#kegiatan'" href="#">Kegiatan</a>
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
          <br/><br/>

          <a href="mailto:clutiksmandayes@gmail.com" class="btn btn-info">Contact Us via Email</a>
      </div>
    </div>

    <br/>
    <div class="container" id="tentang">
      <hr/>
    </div>
    <br/>

    <div class="center">
      <div class="container">
        <h1>Tentang CluTik</h1>
        <br />
        <p>CLUTIK merupakan salah satu ekstrakulikuler di SMAN 2 Mojokerto yang memelajari Ilmu Teknologi dan komputer. Ekstarkulikuer ini banyak diminati para siswa, pasalnya memiliki kegiatan yang atraktif. Pembina yang sabar dan tim yang solid membuat pembelajaran jadi lebih mudah dan menyenangkan. 
<br/> <br/>
Di tahun pembelajaran 2020/2021, CLUTIK membuat inovasi dengan membagi divisi menjadi 3 bagian yakni : NETWORKING, WEB APP DEVELOPMENT dan DESKTOP APP DEVELOPMENT.
<br/>
Di clutik kamu juga akan mendapatkan fasilitas berupa ruangan lab dengan, WI-FI, Komputer, dan tentunya ber AC.
<br/><br/>
Visi CLUTIK : membentuk pribadi yang sadar akan pentingnya penggunaan teknologi informasi dan komunikasi dalam kehidupan sehari-hari.</p>
      </div>
    </div>

    <br/>
    <div class="container" id="kegiatan">
      <hr/>
    </div>
    <br/>

    <div class="center">
      <div class="container">
        <h1>Kegiatan CluTik</h1>
        <div class="row mt-5">
          <div class="col-6 mb-4">
            <img class="img-fluid" height="253" width="450" src="/img/1.jpg">
          </div>
          <div class="col-6">
            <img class="img-fluid" height="253" width="450" src="/img/2.jpg">
          </div>
          <div class="col-6">
            <img class="img-fluid" height="253" width="450" src="/img/3.jpg">
          </div>
          <div class="col-6">
            <img height="253" width="450" src="/img/4.jpg">
          </div>
        </div>
      </div>
    </div>

    <br/>
    <div class="container" id="tentangweb">
      <hr/>
    </div>
    <br/>

    <div class="center" >
      <div class="container">
        <h1>Tentang Website Ini</h1>
        <br>
        <p>Ini adalah sebuah project website opensource dadakan Club TIK SMA Negeri 2 Kota Mojokerto, yang kalian bisa cek langsung public repositorynya di 
          <a class="link" href="https://github.com/ItzMeDwii/clutik-website" target="_blank">https://github.com/ItzMeDwii/clutik-website</a>.</p>
        <br>
          <p>Website ini dibuat oleh:</p>
          <div class="row justify-content-center">
          <div class="col-lg-4 col-sm-6 my-2">
            <a class="link" href="https://github.com/ItzMeDwii/" target="_blank">
        <div class="row d-flex align-items-center border rounded py-2 mx-1 my-1 staff-item">
          <div class="col">
            <h6 class="text-center font-weight-bold pt-2">Satya Bagus Dwiatmaja</h6>
            <p class="text-center">
              Full-stack Developer
            </p>
          </div>
        </div>
        </a>
        </div>

        <div class="col-lg-4 col-sm-6 my-2">
            <a class="link" href="#">
        <div class="row d-flex align-items-center border rounded py-2 mx-1 my-1 staff-item">
          <div class="col">
            <h6 class="text-center font-weight-bold pt-2">Ewaldo Zenobia</h6>
            <p class="text-center">
              Pemberi ide, saran, & penyedia Wi-Fi.
            </p>
          </div>
        </div>
        </a>
        </div>

       <div class="col-lg-4 col-sm-6 my-2">
            <a class="link" href="#">
        <div class="row d-flex align-items-center border rounded py-2 mx-1 my-1 staff-item">
          <div class="col">
            <h6 class="text-center font-weight-bold pt-2">Semua Anggota CluTik</h6>
            <p class="text-center">
              Pemberi saran untuk konten.
            </p>
          </div>
        </div>
        </a>
        </div>

      <div class="col-lg-4 col-sm-6 my-2">
       <a class="link" href="#">
        <div class="row d-flex align-items-center border rounded py-2 mx-1 my-1 staff-item">
          <div class="col">
            <h6 class="text-center font-weight-bold pt-2">Terima kasih juga untuk</h6>
            <p class="text-center">
              Kakak-kakak alumni & Pembina CluTik.
            </p>
          </div>
        </div>
        </a>
        </div>
      </div>

      <br/><br/>
      <p>Website ini dibuat menggunakan:</p>
      <p align="center">
        <img class="mx-3 my-2" alt="Bootstrap" width="64px" src="https://getbootstrap.com/docs/4.5/assets/brand/bootstrap-solid.svg">
        <img class="mx-3 my-2" alt="Vue.js" width="64px" src="https://vuejs.org/images/logo.png">
        <img class="mx-3 my-2" alt="Visual Studio Code" width="64px" src="https://cdn.discordapp.com/attachments/521473681566990340/734078543801221130/download.png">
        <img class="mx-3 my-2" alt="TypeScript" width="64px" src="https://raw.githubusercontent.com/ItzMeDwii/clutik-website/master/src/assets/typescript-logo.png">
        <img class="mx-3 my-2" alt="Sass" width="64px" src="https://sass-lang.com/assets/img/logos/logo-b6e1ef6e.svg">
        <img class="mx-3 my-2" alt="Netlify" width="64px" src="https://www.netlify.com/img/press/logos/logomark.png">
        <img class="mx-3 my-2" alt="Github" width="64px" src="https://github.githubassets.com/images/modules/logos_page/GitHub-Mark.png">
      </p>
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
  // import Slideshow from "@/components/Slideshow.vue";

  /**
   * @Component decorator is used to declare a Vue Component
   * and including Component into the Vue instance
   */
  @Component({
    name: "App",
    components: {
      ThemeChanger,
      // Slideshow
    }
  })
  export default class App extends Vue {
  }
</script>
