<template>
    <div id="header">
        <div id="logo"><a href="#"><svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 74.38 31"><defs></defs><g id="Calque_2" data-name="Calque 2"><g id="Calque_1-2" data-name="Calque 1"><text class="cls-1" transform="translate(0 18.02)">Pu<tspan class="cls-2" x="29.17" y="0">r</tspan><tspan class="cls-3" x="39.38" y="0">ple</tspan></text><text class="cls-4" transform="translate(19.43 25.28)">Pill</text></g></g></svg></a></div>
        <div id="mobile-nav">

            <input type="checkbox" id="menu-toggle">
            <label id="trigger" for="menu-toggle"></label>
            <label id="burger" for="menu-toggle"></label>
            <ul id="menu">
                <li><a href="#">Accueil</a></li>
                <li><a href="#">Développement Web</a></li>
                <li><a href="#">Portfolio</a></li>
                <li><a href="#">A propos</a></li>
                <li><a href="#">Contact</a></li>
            </ul>
        </div>
        <div id="desktop-nav">
            <ul id="desktop-nav-list">
                <li><a href="#">Projets</a></li>
                <li><a href="#">A propos</a></li>
                <li><a href="#" id="btn-contact">Contactez-moi</a></li>
            </ul>
        </div>
    </div>
</template>

<script>
    export default {
        name: "Header"
    }
</script>

<style scoped>

    #logo .cls-1{font-size:21px;fill:#fff;font-family:Arial-Black, Arial;}.cls-2{letter-spacing:0.04em;}.cls-3{letter-spacing:0em;}.cls-4{font-size:18px;fill:#9e16ba;font-family:Akira, Akira;}

    @keyframes checked-anim {
        50% {
            width: 3000px;
            height: 3000px;
        }
        100% {
            width: 100%;
            height: 100%;
            border-radius: 0;
        }
    }
    @keyframes not-checked-anim {
        0% {
            width: 3000px;
            height: 3000px;
        }
    }
    header{
        position: fixed !important;
        z-index: 20;
    }
    #mobile-nav li, a {
        margin: 75px 0 -55px 0;
        color: white;
        font: 14pt "Roboto", sans-serif;
        font-weight: 700;
        line-height: 1.8;
        text-decoration: none;
        text-transform: none;
        list-style: none;
        outline: 0;
        display: none;
    }
    #mobile-nav  li {
        width: 230px;
        text-indent: 56px;}
    #mobile-nav  a:focus {
        display: block;
        color: #333;
        background-color: #eee;
        transition: all .5s;
    }
    #mobile-nav  aside {
        position: absolute;
        color: white;
        top: 35%;
        right: 10%;
        text-align: right;
    }
    #mobile-nav  h1 {
        line-height: 0;
        font-size: 4vw;
        font-weight: 700;
    }
    #mobile-nav  h3 {
        float: right;
        line-height: .3;
        font-size: 2.5vw;
        font-weight: lighter;
    }
    #mobile-nav h4 {
        float: left;
        margin-left: -2%;
        font-size: 1.5vw;
        font-weight: lighter;
    }

    #trigger, #burger, #burger:before, #burger:after {
        position: absolute;
        top: 25px;
        left: 25px;
        background: white;
        width: 30px;
        height: 5px;
        transition: .2s ease;
        cursor: pointer;
        z-index: 1;
        border-radius: 5px;
    }
    #trigger {
        height: 25px;
        background: none;
    }
    #burger:before {
        content: " ";
        top: 10px;
        left: 0;
    }
    #burger:after {
        content: " ";
        top: 20px;
        left: 0;
        width: 15px;
    }
    #menu-toggle:checked + #trigger + #burger {
        top: 35px;
        transform: rotate(180deg);
        transition: transform .2s ease;
    }

    #menu-toggle:checked + #trigger + #burger:before {
        width: 20px;
        top: -2px;
        left: 18px;
        transform: rotate(45deg) translateX(-5px);
        transition: transform .2s ease;
    }
    #menu-toggle:checked + #trigger + #burger:after {
        width: 20px;
        top: 2px;
        left: 18px;
        transform: rotate(-45deg) translateX(-5px);
        transition: transform .2s ease;
    }
    #menu {
        position: fixed;
        margin: 0; padding: 0;
        width: 110px;
        height: 110px;
        border-bottom-right-radius: 100%;
        animation: not-checked-anim .2s both;
        transition: .2s;
        background-color: #130017;
    }
    #menu-toggle:checked + #trigger + #burger + #menu {
        animation: checked-anim 1s ease both;
    }
    #menu-toggle:checked + #trigger ~ #menu > li, a {
        display: block;
    }
    [type="checkbox"]:not(:checked), [type="checkbox"]:checked {
        display: none;
    }


    #logo{
        width: 100%;
        position: fixed;
        top: 21px;
        display: flex;
        justify-content: center;
        align-items: center;
        z-index: 19;
    }
    svg{
        width: 100px;
    }
    svg .cls-1{
        font-family: ArialBlack;
    }


    #desktop-nav{
        width: 100%;
        position: fixed;
        top: 21px;
        display: flex;
        justify-content: flex-end;
    }
    #desktop-nav-list{
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        list-style: none;
        width: 40%;
    }
    #desktop-nav-list li{
        display: block;
    }
    #desktop-nav-list li #btn-contact{
        background: #DE38FF;
        padding: 5px 25px;
        border-radius: 30px;
    }
    #desktop-nav-list li a{
        color: white;
        outline: none;
    }
    #mobilemenu{
        display: flex;
        flex-direction: row;
        align-items: center;
        position: fixed;
        bottom: 0;
        z-index: 1;
        width: 100%;
    }
    .menu-box{
        font-family: ArialBlack;
        font-size: 18px;
        display: block;
        width: 100%;
    }

    .menubox1{
        background: #6f42c1;
        width: 100%;
        text-align: center;
        color: white;
    }
    .menubox2{
        background: white;
        color: #6f42c1;
        width: 100%;
        text-align: center;
    }
    .menubox3{
        background: #6f42c1;
        width: 100%;
        text-align: center;
        color: white;
    }
    .menubox1 a{
        padding: 10px 0;
    }
    .menubox2 a{
        color: #6f42c1;
        padding: 10px 0;
    }
    .menubox3 a{
        padding: 10px 0;
    }

</style>