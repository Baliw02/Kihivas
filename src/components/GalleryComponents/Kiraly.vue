<template>
<div class="full-flex">
    <div class="left-flex">
        <carousel
            :paginationEnabled="true"
            :paginationActiveColor="'#35254d'"
            :paginationColor="'#000000'"
            :paginationPadding="2"
            :per-page="1"
            :touchDrag="false"
            :centerMode="true"
            :spacePadding="0"
        >
            <slide>
                <img src="./Images/kiraly01.jpg">
            </slide>
            <slide>
                <img src="./Images/kiraly02.jpg">
            </slide>
            <slide>
                <img src="./Images/kiraly03.jpg">
            </slide>
            <slide>
                <img src="./Images/kiraly05.jpg">
            </slide>         
            <slide>
                <img src="./Images/kiraly06.jpg">
            </slide>         
        </carousel>
  </div>
  <div class="right-flex" >
    <h1><strong>Király</strong></h1>
    <p>
        A történelmi múltú Király dűlőben 3 hektáros összefüggő szőlőterület található, 2,4 m x 0,9 m-es térállással. A parcella 1 hektár furmint, 
        1 hektár hárslevelű és 1 hektár sárgamuskotály szőlőfajtának ad otthont. Mád legmagasabb vulkanikus hegyének derekán található az impozáns 
        ültetvény, melynek talajában riolittufa és agyag keveréke található. A 25 éves múltra visszatekintő szőlőtőkék gyökérzete az utóbbi időben 
        kezdi elérni azt az ideális nagyságot és
         mélységet, ahonnan a talajban megbújó ásványoknak köszönhetően nagyon komplex szőlőbogyót tud érlelni.
    </p>
  </div>
</div>


</template>

<script>
    export default{
        name:"Kiraly"
    }


</script>

<style scoped>
    .VueCarousel-slide{
        position:relative;
    }
    .VueCarousel{
        width:100%;
        display:flex;
}
   
    .full-flex{
        width: 100%;
        display: flex;
        flex-wrap: nowrap;
    }
    .left-flex{
        margin-left:0;
        justify-content: left;
        width:60%;
        flex:60%;
    }
    .right-flex{
        justify-content: center;
        flex:40%;
        width:40%;
        padding-left: 5%;
        padding-right: 10%;
    }
    img{
        max-width:100%;
    }
    p{
        padding-right: 150px;
        font-weight: 300;
        font-size: medium;
        text-align: justify;
        line-height: 2;
    }
    h1{
        color:black;
        font-size: xx-large;
        width: fit-content;
        border-bottom: 1px solid black;
    }
    @media only screen and (max-width: 812px) {
        .full-flex{
            padding: 1%;
            flex-wrap: wrap;
        }
         .left-flex{
            flex:100%;
        }
        .right-flex{
            flex:100%;
            padding-left: 0;
            padding-right: 0;

         }
        p{
                padding-left:5px;
                padding-right: 5px;
        }
        }
        @media only screen and (max-width: 1280px) {
                        p{
                font-size: small;
                padding-left: 5px;
                padding-right: 5px;
            }
        }


</style>