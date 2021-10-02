<script>
    import {BANNER_1, BANNER_2, BANNER_3, BANNER_4, BANNER_5} from "../../helpers/StaticImageReferencer.svelte"

    let hovered = 3;
</script>

<header>
    <div class="{hovered === 1 ? 'active' : 'nonactive'} imgcontainer d-lg-block d-none"
         on:mouseenter={() => hovered = 1}>
        <img alt="Banner 1"
             src="{BANNER_1}">
        <div class="overlay">

        </div>
    </div>
    <div class="{hovered === 2 ? 'active' : 'nonactive'} imgcontainer" on:mouseenter={() => hovered = 2}>
        <img alt="Banner 2"
             src="{BANNER_2}">
        <div class="overlay">

        </div>
    </div>

    <div class="{hovered === 3 ? 'active' : 'nonactive'} imgcontainer" on:mouseenter={() => hovered = 3}>
        <img alt="Banner 3"
             src="{BANNER_3}">
        <div class="overlay">

        </div>
    </div>

    <div class="{hovered === 4 ? 'active' : 'nonactive'} imgcontainer" on:mouseenter={() => hovered = 4}>
        <img alt="Banner 4"
             src="{BANNER_4}">
        <div class="overlay">

        </div>
    </div>

    <div class="{hovered === 5 ? 'active' : 'nonactive'} imgcontainer d-lg-block d-none"
         on:mouseenter={() => hovered = 5}>
        <img alt="Banner 5"
             src="{BANNER_5}">
        <div class="overlay">

        </div>
    </div>


    <div class="position-absolute bottom-0 start-50 translate-middle w-100 pb-5 pb-lg-3">
        <h1>
            Clarissa Punipun Fan-Concept Website
        </h1>
        <h1>
            クラリッサ プニプン
        </h1>
    </div>
</header>


<style>
    h1 {
        text-align: center;
        margin: 0;
        text-transform: uppercase;
        text-shadow: 2px 2px 5px black;
        color: white;
    }

    header {
        height: 100vh;
        background: linear-gradient(0deg, rgba(53, 19, 108, 1) 0%, rgba(53, 19, 108, .8) 100%);
        display: flex;
        justify-content: center;
        align-items: center;
        position: relative;
    }

    .imgcontainer {
        height: 100%;
        transition: all .15s ease-in-out;
        position: relative;
    }

    .overlay {
        position: absolute;
        left: 0;
        top: 0;
        width: 100%;
        height: 100%;
        transition: all .25s ease-in-out;
        display: flex;
        flex-direction: column;
    }

    .overlay:hover {
        background: transparent;
    }

    .imgcontainer.active {
        width: 40%;
    }

    .imgcontainer.nonactive {
        width: 15%;
    }

    img {
        object-fit: none;
        object-position: 50% 0;
        height: 100%;
        width: 100%;
        position: relative;
    }

    @media (max-width: 1200px) {
        .imgcontainer.active {
            width: 60%;
        }

        .imgcontainer.nonactive {
            width: 20%;
        }
    }
</style>