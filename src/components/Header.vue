<template>
    <header>
        <MenuList/>
    </header>
</template>
<script>
import MenuList from './Menulist'

    export default{
        name:"Header",
        components:{
        MenuList

    },
    }
    
</script>
<style scoped>
    header{
        text-align: center;
        align-items: center;
        top:0;
        left:0;
        right: 0;
        width: 100%;
        position: relative;
        background-color: black;
        color:black;
        margin-bottom: 0;
        z-index: 999;
        height: 100px;
    }
</style>