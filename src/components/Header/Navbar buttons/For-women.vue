<template>
    <div class="for-women">
        <div class="container">
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>
.for-women{
    position: absolute;
    width: 1140px;
    top: 50px;
    left: -512px;
    height: 345px;
    display: flex;
    justify-content: center;
}
.container{
    position: relative;
    width: 100%;
    height: 345px;
    background-color: darkorchid;
}
.container:after{
    content: '';
    position: absolute;
    width: 20px;
    height: 20px;
    transform: rotate(45deg);
    background-color:darkorchid;
    top: -7px;
    left: 48.3%;
}
.container:before{
    content: '';
    position: absolute;
    width: 80px;
    height: 80px;
    top: -30px;
    left: 45%;
}
</style>
