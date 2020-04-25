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
    width: 100%;
    top: 115px;
    height: 345px;
    left: 0;
    display: flex;
    justify-content: center;
}
.container{
    position: relative;

    width: 1140px;
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
</style>
