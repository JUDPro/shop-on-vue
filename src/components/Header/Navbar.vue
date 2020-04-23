<template>
    <div id="navbar">
        <div class="navbox">
            <div class="posbox">
                <div class="contact box">
                    <i class="fa fa-phone" aria-hidden="true"></i>
                    <div class="number">(00)-123-456-789</div>
                    <i class="fa fa-envelope" aria-hidden="true"></i>
                    <div class="mail">weshop@gmail.com</div>
                </div>
                <div class="search box">
                    <div class="form">
                        <input type="text" name="search" autocomplete="off" required/>
                        <label for="search" class="label-search">
                            <!--span class="content-search">Search</span-->
                            <span class="fa fa-search fa-xs my-fix-search-icon"></span>
                        </label>
                    </div>
                </div>
                <div class="other box">
                    <div class="lang btn-o">English<i class="fa fa-sort-down" aria-hidden="true"></i></div>
                    <div class="usd btn-o">USD<i class="fa fa-sort-down" aria-hidden="true"></i></div>
                    <div class="login btn-o">Login</div>
                </div>
            </div>
            <div class="posbox">
                <div class="box">
                    <div class="logo">
                        <div class="text-logo">weshop</div>
                    </div>
                </div>
                <div class="for-button box">
                    <div class="btn home">Home</div>
                    <div class="btn shop">Shop<i class="fa fa-sort-down" aria-hidden="true"></i></div>
                    <div class="btn men">Men<i class="fa fa-sort-down" aria-hidden="true"></i>
                        <forMen></forMen>
                    </div>
                    <div class="btn women">Women<i class="fa fa-sort-down" aria-hidden="true"></i></div>
                    <div class="btn page">Page<i class="fa fa-sort-down" aria-hidden="true"></i></div>
                    <div class="btn blog">Blog</div>
                    <div class="btn contactus">Contact us</div>
                </div>
                <div class="cash box">
                    <div class="border-for-cash">
                        <i class="fa fa-shopping-bag"></i>
                        <div class="Number-of-goods">2</div>
                    </div>
                    <div class="cash-text">$25.00</div>
                </div>
            </div>
        </div>
    </div>
</template>

<script>
import forMen from './Navbar buttons/For-men.vue'
export default {
    components:{
      forMen
    }
}
</script>

<style scoped>
@import "../fonts/fontawesome-free-5.13.0-web/css/all.css";

#navbar{/*стили для навигационной панели*/
    height: 120px;
    background-color: #48689a;
    display: flex;
    justify-content: center;
    font-family: "Font Awesome 5 Free", RobotoSlab;
}
/*-----------------------------------*/

/*Нужное позиционирование*/
.navbox{
    height: 105px;
    width: 1140px;
    display: flex;
    flex-direction: column;
    padding-left: 15px;
    padding-right: 15px;
}
.box{
    width: 20%;
    height: 100%;
}
.posbox{
    height: 50%;
    width: 100%;
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
}
/*-----------------------------------*/

/*Позиционирование верхних элементов*/
.search{
    flex-grow: 1;
    display: flex;
    justify-content: space-around;
    flex-direction: column;
    align-items: center;
    width: 300px;
    background-color: unset;
}
.form{
    width: 50%;
    position: relative;
    padding-top: 20px;
    height: 25px;
    overflow: hidden;
}
.form input{
    background-color: #48689a;
    width: 100%;
    height: 100%;
    color: white;
    border: none;
    outline: none;
}
.form label{
    position: absolute;
    bottom: 0px;
    left: 0%;
    height: 100%;
    width: 100%;
    pointer-events: none;
    border-bottom: 1px solid white;
}
.form label::after{
    content: "";
    position: absolute;
    left: -1px;
    bottom: -1px;
    height: 100%;
    width: 100%;
    border-bottom: 2px solid white;
    transform: translateX(-100%);
    transition: all 0.3s ease;
}
.content-search{
    position: absolute;
    bottom: 5px;
    left: 0px;
    transition: all 0.3s ease;
    color: white;
}
.form input:focus + .label-search .content-search, 
.form input:valid + .label-search .content-search{
    transform: translateY(-120%)scale(0.9);
    font-size: 12px;
    color: white;
}
.form input:focus + .label-search::after,
.form input:valid + .label-search::after{
    transform: translateX(0%);
    left: 0px;
}
.my-fix-search-icon{
    position: absolute;
    bottom: 5px;
    right: 0px;
    color: white;
}
/*Конец для поиска :D*/
.contact{
    width: 22%;
    color: white;
    display: flex;
    flex-wrap: nowrap;
    justify-content: space-between;
    font-size: 12px;
    align-items: center;
}
.fa-phone{
    transform: rotate(90deg);
    font-size: 10px;
}
.other{
    display: flex;
    justify-content: space-around;
    color: white;
    align-items: center;
    font-size: 12px;
}
.btn-o{
    display: flex;
    padding: 5px;
    cursor: pointer;
}
.btn-o:hover{
    background-color: #466392;
}
.fa-sort-down{
    padding-left: 5px;
}
/*-----------------------------------*/

/*Позиционирование нижних элементов*/
/*Для лого*/
.logo{
    width: 160px;
    border-style: solid;
    border-color: #00cdc6;
}
.text-logo{
    font-size: 35px;
    font-family: 'Oswald DemiBold';
    text-align: center;
    color: #00cdc6;
    line-height: 39px;
    padding-bottom: 8px;
}

/*Для кнопок*/
.for-button{
    flex-grow: 1;
    display: flex;
    justify-content: space-evenly;
    flex-wrap: wrap;
    align-content: center;
}
.btn{
    display: flex;
    font-size: 14px;
    color: white;
    padding: 10px;
    margin-top: 10px;
    cursor: pointer;
}
.btn:hover{
    background-color: #466392;
}

/*Для корзины и ценника*/
.cash{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-wrap: wrap;
    position: relative;
}
.border-for-cash{
    width: 37px;
    height: 37px;
    border: 1px solid;
    border-color: white;
    border-radius: 25px;
    position: relative;
}
.fa-shopping-bag{
    color: white;
    position: absolute;
    top: 10px;
    left: 11px;
}
.Number-of-goods{
    position: absolute;
    right: -5px;
    top: -3px;
    height: 18px;
    width: 18px;
    border-radius: 25px;
    background-color: white;
    color: #48689a;
    text-align: center;
    font-size: 12px;
}
.cash-text{
    color: white;
    font-size: 14px;
    font-family: "Font Awesome 5 Free", RobotoSlab;
    padding-left: 15px;
}
/*-----------------------------------*/
</style>