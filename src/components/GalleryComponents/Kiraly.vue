<template>
<section>
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
            @page-change="counter+=1"
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
<div class="visible" id="coupon-box"  v-if="counter >= 3 && counter < 4">

    <div class="info">
    <h1>gratulálunk</h1>
    <span id="coupon-info">
        Mivel ilyen szorgosan gyüjtöd az információt, meg jutalmazunk egy kóddal
        melyet beváltva minden termékünk árából levon 10%-ot!
    </span>
    <br>
    <span id="coupon-code">
        Kód: sd52a4
    </span>
    </div>
</div>
</section>
</template>

<script>
    export default{
        name:"Betsek",
        data(){
            return{
                counter:0
            }
        }
        
    }


</script>

<style lang="scss" scoped>
    $sec: rgba(72, 61, 139, 100%);
    $prim: white;

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
        margin-bottom: 5%;
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
    .visible{
        margin: auto;
        display:block;
        width:50%;
        padding:10px 10px;
        background-color: $sec;
    }
    .info{
        justify-content: left;
        font-family: Roboto;
        width:50%;
        margin:auto;
        color:white;
    }
    .info > h1{
        margin:auto;
        color:white;
        border-bottom:3px solid white;
        font-size: x-large;
        text-transform: uppercase;
        font-weight: 800;
    }
    #coupon-info{
        font-size: medium;
        line-height: 1.5;
        font-weight: 300;
    }
    #coupon-code{
        background-color: $prim;
        color:$sec;
        font-size: xx-large;
        text-transform: uppercase;
        padding:0;
    }
    @media only screen and (max-width: 1215px) {
        .visible{
        width:100%;
        }
        #coupon-code{
            font-size: x-large;
        }
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
        @media only screen and (max-width: 1300px) {
                        p{
                font-size: small;
                padding-left: 5px;
                padding-right: 5px;
            }
        }
        @media only screen and (max-width: 1647px) {
                        p{
                font-size: medium;
                padding-left: 5px;
                padding-right: 5px;
            }
        }
        @media only screen and (max-width: 360px) {
            p{
                line-height: 1.5;
            }
        }


</style>