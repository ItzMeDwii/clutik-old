<!--
 * Welcome to Clovuer
 * The comments in each files will guide you through your very cool journey
 * discovering what Vue can do.
 -->
<template>
<div id="yes" class="mt-5">
<button class="btn btn-dark float-left" onclick="plusDivs(-1)"><i class="fas fa-angle-double-left fa-lg"></i></button>
<button class="btn btn-dark float-right"  onclick="plusDivs(+1)"><i class="fas fa-angle-double-right fa-lg"></i></button>
    <div id="slideshow">
    </div>
    </div>
</template>

<script lang="js">
    import Vue from "vue"
    import {Component} from "vue-property-decorator";
    @Component({
        name: "Slideshow",
        async mounted() {

            //async function getImage() {
            //const num = Math.random() * (16 - 1) + 1; 
            //document.getElementById("slideshow").innerHTML = "<img id='"+ num.toFixed(0) +"' src='https://dwii.me/clutik/assets/"+ num.toFixed(0) +".jpg'>";
            //return console.log("a");
            //}

            //setInterval(await getImage(), 1000);
            
            const arrey = [];

            for (let i = 1; i < 17; i++) {

            arrey.push("<img class='slideimages' width='80%' src='https://dwii.me/clutik/assets/"+ i +".jpg'>");

            }

            document.getElementById("slideshow").innerHTML = arrey.join("")


                  let slideIndex = 1;
      
      function showDivs(n) {
        let i;
        const x = document.getElementsByClassName("slideimages");
        if (n > x.length) {slideIndex = 1}
        if (n < 1) {slideIndex = x.length}
        for (i = 0; i < x.length; i++) {
          x[i].style.display = "none";
        }
        x[slideIndex-1].style.display = "block";
        
      }
      
      
      showDivs(slideIndex);


        }
    })
    export default class Slideshow extends Vue {
    }
</script>
