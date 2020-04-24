<template>
    <div class="goods">
        <div class="container">
            <div class="content">
                <div class="product">
                    <img src="https://sun9-20.userapi.com/c857016/v857016902/d0916/unoNMEedTfg.jpg" alt="image">
                    <div class="info-box">
                        <div class="name">Denim t-shirt For Boys</div>
                        <div class="cash">$289 - $250</div>
                    </div>
                </div>
                <div class="product">
                    <img src="https://sun9-20.userapi.com/c857016/v857016902/d0916/unoNMEedTfg.jpg" alt="image">
                    <div class="info-box">
                        <div class="name">Denim t-shirt For Boys</div>
                        <div class="cash">$289 - $250</div>
                    </div>
                </div>
            </div>
            <div class="button">
                <div class="btn continue">CONTINUE SHIPPING</div>
                <div class="btn procced">PROCCED TO CHECKOUT</div>
            </div>
        </div>
    </div>
</template>
<script>
export default {}
</script>
<style scoped>
.goods{
    background-color: white;
    position: absolute;
    height: 435px;
    width: 360px;
    top: 63px;
    left: -150px;
    box-shadow: 0px 1px 12px -3px;
    display: flex;
    align-items: center;
    justify-content: center;
}
.goods:after{
    content: '';
    position: absolute;
    width: 20px;
    height: 20px;
    background-color: white;
    top: -5px;
    right: 116px;
    transform: rotate(45deg);
}
.container{
    width: 300px;
    height: 350px;
    display: flex;
    justify-content: center;
    flex-direction: column;
    align-items: center;
}
/*Для товаров*/
.content{
    width: 100%;
    height: 220px;
    display: block;
}
.product{
    height: 85px;
    width: 100%;
    display: flex;
    margin-bottom: 20px;
    border-bottom: 1px solid rgba(139, 139, 139, 0.5);
}
img{
    width: 65px;
    height: 65px;
}
.info-box{
    position: relative;
    height: 75px;
    left: 15px;
}
.cash{
    position: relative;
    top: 10px;
    color: #48689a;
}
/*--------------------------------*/

/*Для кнопок*/
.button{
    width: 100%;
    height: 140px;
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-evenly;
}
.btn{
    height: 50px;
    font-size: 14px;
    display: flex;
    align-items: center;
    justify-content: center;
    cursor: pointer;
}
.continue{
    width: 296px;
    border: 2px solid #48689a;
    color: #48689a;
}
.continue:hover{
    width: 294px;
    border: 3px solid #466392;
    color: #466392;
    font-size: 15px;
}
.procced{
    width: 300px;
    background-color: #48689a;
    color: white;
}
.procced:hover{
    background-color: #466392;
    font-size: 15px;
}
/*--------------------------------*/
</style>