<template>
    <div class="full-sec">
        <div class="text-box">
            <div class="text-in">
            <h1>A terület</h1>
            <p>
                A Juliet Victor számára a világhírű Tokaji borvidék szívében található Mád történelmi községe tökéletes éghajlati feltételeket, termőtalajt és bortermelő területet biztosít, amely az egyedülálló erjesztési és érlelési folyamatok képességének, mesterségbeli tudásának is táptalajává válik.

            </p>
            </div>
        </div>
    </div>
</template>

<script>
    export default{
        name:"SectionThree",
    }
</script>

<style lang="scss" scoped>
    .full-sec{
        z-index: 10;
        width: 100%;
        margin-top: 15%;
        display: block;
        background-image: url("./backthird.jpg");
        background-size: 80%;
        background-repeat: no-repeat;
        background-position: right;
        height: 600px;
    }
    .text-box{
        top:-10%;
        position: relative;
        width:100%;
        margin-left: 10%;
        margin-bottom: 20%;
    }
    .text-in{
        width:30%;
        background-color: rgba(72, 61, 139, 100%);
        text-align: left;
        padding:100px 60px;
    }
    h1{
        color:white;
        border-bottom:1px solid white;
        width: fit-content;
        font-size: xx-large;
        font-weight: 700;
    }
    p{
        font-size: medium;
        color:white;
        line-height: 2;
        font-family: Roboto;
    }
    @media only screen and (max-width: 1054px) {
        .full-sec{
            background-position: center;
            background-size: 100%;
                        }
        .text-in{
            width: 80%;
        }
                   
        }
    @media only screen and (max-width: 651px) {
        h1{
            font-size: medium;
        }
        p{
            font-size: small;
        }
        .full-sec{
            margin-bottom: 5%;
            margin-top: 60%;
        }
        .text-box{
            padding:30px 30px;
            padding-bottom:30px;
            margin-left:0%;
            margin-right: 0%;
            top:-30%;
        }
        .text-in{
            padding:50px 50px;
            width:100%;
        }
        }
</style>