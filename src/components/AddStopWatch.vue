<template>
    <div class="main">
        <button id="add" @click="add"></button>
    </div>
</template>

<script>
    export default {
        
    }
</script>

<style scoped>
    .main{
        width: 255px;
        height: 120px;
        background-color: #696969;
        display: flex;
        justify-content: center;
        align-items: center;
    }
    #add{
        background: #9E9E9E;
        height: 20px;
        position: relative;
        border: 0px;
        width: 3px;
    }
    #add:after{
        background: #9E9E9E;
        content: "";
        height: 3px;
        left: -8.5px;
        position: absolute;
        top: 8.5px;
        width: 20px;
    }
    #add:hover{
        background: #ffffff;
    }
    #add:hover::after{
        background: #ffffff;    
    }
</style>