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
                <img src="./Images/betsek2.jpg">
            </slide>
            <slide>
                <img src="./Images/betsek3.jpg">
            </slide>
            <slide>
                <img src="./Images/betsek4.jpg">
            </slide>
            <slide>
                <img src="./Images/betsek5.jpg">
            </slide>         
        </carousel>
  </div>
  <div class="right-flex" >
    <h1><strong>Betsek</strong></h1>
    <p>
        A varázslatos hangulatú Betsek dűlőben 3 hektáron, 3,2 m x 1 m-es térállású 40 éves múltra visszatekintő szőlő található. A széles sortávolságnak és a déli lejtésű soriránynak köszönhetően a nap a legideálisabban fejti ki energiáit a szőlőtőkékre, így a dűlők közül 
        itt beszélhetünk a legkorábban érő ültetvényről. 
        A fehér riolittufa kőzetének köszönhetően kimagaslóan 
        ásványos, komplex termés szüretelhető. Az ültetvényen törzsfelújítást alkalmaztunk az elöregedett termőalapok megmentése érdekében. Ez a különleges hely a bölcsője a dűlőről elnevezett, egyik 2017-es, élettel teli, kifinomult zamatú és fűszerességű furmintunknak.
    </p>
  </div>
</div>


</template>

<script>
    export default{
        name:"Betsek"
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