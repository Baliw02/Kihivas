<template>
    <div class="First-Content">
        <h1>A birtok</h1>
    </div>
</template>

<script>
    export default{
        name: "FirstContent",
    }
</script>

<style lang="scss" scoped>
$font-f: Fortlight;
$font-l: white;
$font-d: black;
$font-w: 600;
$h1-s: xx-large;

.First-Content{
    animation-name: fade-in;
    animation-duration: 3s;
    animation-direction: normal;
    float:inline-end;
    clear:none;
    width:100%;
    background-image: url("./backfirst.jpg");
    height: 700px;
    background-attachment: fixed;
    background-position: center;
    background-repeat: no-repeat;
    background-size: cover;
    }
h1{
    animation-name: fly;
    animation-duration: 2s;
    font-weight: $font-w;
    margin-top: 22%;
    color:$font-l;
    font-size: 50px;
    font-family: $font-f;
    }
@media only screen and (max-width: 455px) {
    .First-Content{
        height: 450px;
    }
    h1{
        margin-top: 50%;
        font-size: $h1-s;
        }
    }

@keyframes fade-in {
    from{
        filter:brightness(0);
    }
    to{
        filter:brightness(1)
    }
}
@keyframes fly{
    from{
        transform:translateX(-200%);
    }
    to{
        transform:translateX(0);
    }
}
</style>

