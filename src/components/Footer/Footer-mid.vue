<template>
    <div class="container">
        <div class="top"></div>
        <div class="bot">
            <div class="social">

            </div>
        </div>
    </div>
</template>

<script>
export default {}
</script>

<style scoped>

.container{
    position: relative;
    height: 465px;
    width: 100%;
}
.top{
    width: 100%;
    height: 360px;
}
.bot{
    width: 100%;
    height: 105px;
    display: flex;
    justify-content: center;
    align-items: center;
}
.social{
    width: 250px;
    height: 75px;
    border-bottom: 1px solid rgba(139, 139, 139, 0.5);
}
img{
    width: 10px;
    height: 10px;
}
</style>