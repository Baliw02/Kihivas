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
        left:0;
        top:0;
        width: 100%;
        position: fixed;
        background-color: black;
        color:black;
        margin-bottom: 0;
        z-index: 999;
        height: 100px;
    }
</style>