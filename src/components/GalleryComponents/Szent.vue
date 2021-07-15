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
                <img src="./Images/tamas01.jpg">
            </slide>
            <slide>
                <img src="./Images/tamas02.jpg">
            </slide>
            <slide>
                <img src="./Images/tamas03.jpg">
            </slide>
            <slide>
                <img src="./Images/tamas04.jpg">
            </slide>         
        </carousel>
  </div>
  <div class="right-flex" >
    <h1><strong>Szent-Tamás</strong></h1>
    <p>       
        Mád egyik legkomplexebb ásványi anyag összetételű dűlőjében, a Szent Tamás Dűlőben 0,4 hektár 
        2,4 m x 1 m-es térállású ültetvényünk található. A régmúltba visszatekintő, 1962-es ültetés ellenére 98 
        %-ban eredeti furmint és hárslevelű tőkékkel rendelkezik a terület. A talaj felső rétege vörösagyag, amely 
        3 m vastagságban helyezkedik el a felszínen és az ezt követő altalaj pedig egybefüggő zeolit réteg. A sorokon végigsétálva 
        az öreg tőkékre jellemző nyugodtság hatása érzékelhető - apró laza fürtök, vékonyabb hajtások jellemzőek ezen a különleges termőterületen.
    </p>
  </div>
</div>


</template>

<script>
    export default{
        name:"Szent"
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