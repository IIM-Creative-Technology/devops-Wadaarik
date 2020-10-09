<template>
    <div id="firstpage">
        <div id="top-website">
            <div id="top-contain">
                <h1>Nicolas Boudier</h1>
                <h2 class="big-title">Je donne vie à votre projet</h2>
                <h2 class="poste-desktop">Développeur Web - Chef de projet Digital</h2>
                <h2 class="poste-mobile">Développeur Web<br>Chef de projet Digital</h2>
                <span class="underline"></span>
            </div>
            <a href="#" id="mes-projets">Mes projets</a>
        </div>
        <div id="mes-competences">
            <div class="title">
                <h2>Mes compétences</h2>
                <span class="underline"></span>
            </div>
            <div class="glider-contain">
                <div class="glider draggable">
                    <div class="glider-track" style="width: 900px;"><div class="glider-slide active center" style="height: auto; width: 300px;"><img src="../../img/developpement-web-purplepill.png" title="developpement-web-purplepill" alt="Développement Web"></div><div class="glider-slide center" style="height: auto; width: 300px;"><img src="img/gestion-de-projet-purplepill.png" title="gestion-de-projet-purplepill" alt="Gestion de projet"></div><div class="glider-slide right-1" style="height: auto; width: 300px;"><img src="img/analytics-seo-purplepill.png" title="analytics-seo-purplepill" alt="Analytics SEO"></div></div></div>
                <button class="glider-prev" style="outline: none">«</button>
                <button class="glider-next" style="outline: none">»</button>
            </div>
            <div class="competences-row">
                <ul>
                    <li><img src="../../img/developpement-web-purplepill.png" title="developpement-web-purplepill" alt="Développement Web"></li>
                    <li><img src="../../img/gestion-de-projet-purplepill.png" title="gestion-de-projet-purplepill" alt="Gestion de projet"></li>
                    <li><img src="../../img/analytics-seo-purplepill.png" title="analytics-seo-purplepill" alt="Analytics SEO"></li>
                </ul>
            </div>
        </div>
        <div id="a-propos">
            <div id="first-column">
                <div class="title">
                    <h2>A propos</h2>
                    <span class="underline"></span>
                </div>
                <div class="text-section">
                    <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Praesent ut mollis arcu. Aenean ut tortor et velit ornare pulvinar. Suspendisse ut turpis et nibh condimentum finibus. Integer ligula diam, vehicula ac nulla nec, venenatis mollis purus. Maecenas vitae mi a orci scelerisque euismod. Maecenas consectetur, enim eu hendrerit sagittis, purus quam consectetur purus, sed dignissim neque mi in mauris. Praesent fermentum viverra tortor cursus vulputate. Aenean semper massa tempor sagittis bibendum. Pellentesque consequat odio at nulla aliquam feugiat a eu lacus. Quisque porta mauris at nisi fringilla, id placerat nibh faucibus. Duis et feugiat ante, quis interdum lectus. Praesent accumsan convallis libero, in pharetra tortor luctus sit amet. Phasellus in sapien a augue maximus mollis eu nec ipsum. Sed ullamcorper nunc orci, sed fringilla eros vulputate ac. Maecenas eu sapien id orci eleifend posuere.
                    </p>
                    <div id="select-btn">
                        <a href="#">Mes projets</a>
                    </div>
                </div>
            </div>
            <img src="../../img/a-propos-background-purplepill.jpg" title="developpement-web-background-a-propos-purplepill" alt="Développement background section A propos">
        </div>
        <div id="references">
            <div class="title">
                <h2>Mes références</h2>
                <span class="underline"></span>
            </div>
            <div class="glider-contain">
                <div class="glider draggable">
                    <div class="glider-track" style="width: 1068px;">
                        <div class="glider-slide left-1" style="height: auto; width: 356px;"><img src="../../img/expertisme-logo_blanc-purplepill.png" title="expertisme-logo_blanc-purplepill" alt="EXPERT is Me"></div>
                        <div class="glider-slide active center" style="height: auto; width: 356px;"><img src="../../img/5m-ventures-logo-white-purplepill.png" title="5m-ventures-logo-white-purplepill" alt="5M Ventures"></div>
                        <div class="glider-slide right-1" style="height: auto; width: 356px;"><img src="../../img/logo-marque-et-team-purplepill.png" title="logo-marque-et-team-purplepill" alt="Marque et Team" style="width: 190px;"></div>
                    </div>
                </div>
                <button class="glider-prev" style="line-height: 0; outline: none">«</button>
                <button class="glider-next" style="line-height: 0; outline: none">»</button>
            </div>
            <div class="references-row">
                <ul>
                    <li><img src="../../img/expertisme-logo_blanc-purplepill.png" title="expertisme-logo_blanc-purplepill" alt="EXPERT is Me"></li>
                    <li><img src="../../img/5m-ventures-logo-white-purplepill.png" title="5m-ventures-logo-white-purplepill" alt="5M Ventures"></li>
                    <li><img src="../../img/logo-marque-et-team-purplepill.png" title="logo-marque-et-team-purplepill" alt="Marque et Team" style="width: 190px;"></li>
                </ul>
            </div>
        </div>
    </div>

</template>

<script>
    export default {
        name: "firstpage"
    }
</script>

<style scoped>
    #top-website{
        background: url("../../img/background-home-purplepill.png");
        background-position: center;
        background-attachment: scroll;
        background-repeat: no-repeat;
        background-size: cover;
        min-height: 736px;
        width: 100%;
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column;
    }
    #top-contain{
        width: 88%;
    }
    #top-contain h1{
        font-family: ArialBlack;
        font-size: 25px;
        color: #DE38FF;
    }
    #top-contain h2.big-title{
        font-family: ArialBlack;
        font-size: 42px;
        color: white;
    }
    #top-contain .poste-mobile, #top-contain .poste-desktop{
        font-family: ArialBlack;
        font-size: 25px;
        color: #DE38FF;
        text-shadow: none;
    }
    .underline{
        display: block;
        width: 40%;
        max-width: 280px;
        height: 10px;
        background: white;
        box-shadow: 7px 5px #9E16BA;
    }
    #mes-projets{
        padding: 5px 30px;
        border-radius: 30px;
        background: #9E16BA;
        border: none;
        outline: none;
        margin-top: 105px;
        transition-duration: 0.5s;
    }
    #mes-projets:hover{
        background: white;
        color: #9E16BA;
        box-shadow: 7px 7px #9E16BA;
        transition-duration: 0.5s;
    }

    #mes-competences{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    #mes-competences img{
        width: 250px;
    }
    .title{
        width: 88%;
    }
    .title h2{
        font-size: 45px;
        font-weight: 900;
        color: white;
        text-shadow: 4px 4px #9E16BA;
    }
    .title .underline{
        width: 200px;
    }
    .competences-row{
        width: 100%;
        padding: 50px 0;
    }
    .competences-row ul{
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
    }

    #a-propos{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: row;
    }
    #first-column{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    .text-section p{
        color: white;
        width: 88%;
        text-align: justify
    }
    #select-btn{
        width: 88%;
        display: flex;
        justify-content: center;
    }
    #select-btn a{
        padding: 5px 30px;
        border-radius: 30px;
        background: #9E16BA;
        border: none;
        outline: none;
        transition-duration: 0.5s;
    }
    #select-btn a:hover{
        background: white;
        color: #9E16BA;
        box-shadow: 7px 7px #9E16BA;
        transition-duration: 0.5s;
    }
    .text-section{
        display: flex;
        flex-direction: column;
        align-items: flex-start;
        padding: 20px 0;
        width: 88%;
    }
    #a-propos img{
        max-width: 400px;
        position: absolute;
        z-index: -1;
        right: 4%;
        opacity: 0.7;
    }
    #references{
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
    }
    #references img{
        width: 250px;
    }
    .references-row{
        width: 100%;
        padding: 50px 0;
    }
    .references-row ul{
        display: flex;
        flex-direction: row;
        justify-content: space-evenly;
        align-items: center;
    }

    @media screen and (max-width: 766px){
        .poste-desktop{
            display: none !important;
        }
        .competences-row{
            display: none;
        }
        .text-section p {
            width: 100%;
        }
        #select-btn {
            width: 100%;
        }
        #a-propos img{
            display: none;
        }
        .references-row{
            display: none;
        }
    }
    @media screen and (min-width: 767px){
        .poste-mobile{
            display: none !important;
        }
        .glider-contain{
            display: none;
        }

    }
</style>