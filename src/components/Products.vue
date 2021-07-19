<template>
<div class="row">
    <div class="left-flex">
        <img id="wine" src="./Wines/jv_betsek-1-102x300.png">
        <img class="decs" src="./Wines/silver-decanter-2020.png" width="12%">
        <div class="title">
        <h1><strong>Birtok furmint 2017</strong></h1>
        <p id="cat">2017 / SZÁRAZ</p>
        </div>
        <div class="info">
            <p>Kristálytiszta, halvány szalmasárga színét ragyogó, arany villanások nemesítik. Tiszta, visszafogott illatában enyhén fanyar…</p>
            <button>BŐVEBBEN <i class="fa fa-angle-right" aria-hidden="true"></i></button>
        </div>
        <div class="price">
            <p id="price"><strong>{{Wines.birtok_fur}}FT</strong></p>
            <input id="num" type="number">
            <button id="shop"> VÁSÁRLÁS</button> 
        </div>

    </div>
    <div class="right-flex">
        <img id="wine" src="./Wines/estate-furmint-2017-dry-1-1-102x300.png">
        <div class="title">
        <h1><strong>Furmint 2016</strong></h1>
        <p id="cat">2016 / SZÁRAZ</p>
        </div>
        <div class="info">
            <p>Kristálytiszta, ragyogó, szalmasárga színnel rendelkezik. Magas viszkozitása nagy beltartalmi értékről tanúskodik…</p>
            <button>BŐVEBBEN <i class="fa fa-angle-right" aria-hidden="true"></i></button>
        </div>
        <div class="price">
            <p id="price"><strong>{{Wines.betsek_dul}}FT</strong></p>     
            <input id="num" type="number">
            <button id="shop"> VÁSÁRLÁS</button> 
        </div>

    </div>
</div>
    
</template>

<script>
    export default{
        data(){
            return{
                Wines:{
                    birtok_fur: 4990,
                    betsek_dul: 8890
                }
            }
        }
    }
</script>

<style lang="scss" scoped>
    $bgcol: grey;
    $sec: rgba(72, 61, 139, 100%);
    $prim: white;

    h1{
        font-weight: 1000;
        font-family: Fortlight;
        color:black;
        font-size: xx-large;
    }
    .title{
        border-bottom: 1px solid black;

    }
    .row{
        margin-top: 10%;
        margin-left:5%;
        margin-right: 5%;
        align-items: center;
        justify-content: center;
        white-space: wrap;
        padding-bottom:10%;
    }
    .left-flex{
        text-align: left;
        width:500px;
        height:450px;
        background-color: rgba(240,240,240,100%);
        padding-top: 60px;
        padding-bottom: 60px;
        padding-left: 10%;
        padding-right: 5%;
        display: inline-block;
        margin-inline-end: 30%;
        position: relative;
    }
    .right-flex{
        text-align: left;
        padding-top: 60px;
        padding-bottom: 60px;
        height:450px;
        padding-left: 10%;
        padding-right: 5%;
        width:500px;
        background-color: rgba(240,240,240,100%);
        display: inline-block;
        position: relative;
    }
    p{
        text-transform: uppercase;
        line-height: 2;
        font-size: small;
        font-weight: 200;
    }
    button{
        color: $sec;
        background-color: transparent;
        border:none;
    }
    img{
        position:absolute;
        left:-10%;
        top:-5%;
    }
    .decs{
        left:13%;
        top:10%;
    }
    .price{
        height: 10%;
        left:0;
        width: 100%;
        position:absolute;
        bottom:0;
    }
    #price{
        
        position:absolute;
        color:black;
        font-size: medium;
        font-family: Fortlight;
        width:fit-content;
        left:35%;
        font-weight: 500;
    }
    #num{
        width:10%;
        position: absolute;
        left:50%;
    }
    #shop{
        position:absolute;
        left:65%;
        background-color: rgba(72, 61, 139, 100%);
        border-radius: 15px;
        color:white;
        font-size: small;
        font-weight: 700;
        padding:5px 5px;
    }
        @media only screen and (max-width: 1810px) {
            .left-flex{
                width: 100%;
                margin-inline-end: 0;
                margin-bottom: 20%;            
                }
            .right-flex{
                width: 100%;
            }
            #wine{
                left:-8%;
                width:12%;
            }
            .decs{
                top: 0;
                left:3%;
                width: 5%;
            }
        }
        @media only screen and (max-width: 462px) {
            #price{
                left:25%;
            }
            #num{
                width:45px;
                left:45%;
            }
            .decs{
                width:15%;
            }
        }
</style>
