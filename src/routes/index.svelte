<script>
    import HeaderBanner from "../components/index/HeaderBanner.svelte";
</script>

<HeaderBanner/>
<nav>
    <div class="topside">
        <h1>
            Clarissa Punipun Official Website
        </h1>
        <h1>
            クラリッサ プニプン
        </h1>
    </div>
    <div class="botside">
        <a class="nav-item" href="/">Home</a>
        <a class="nav-item" href="#">Shop</a>
        <a class="nav-item" href="#">Events</a>
        <a class="nav-item" href="#">Games & Equipments</a>
        <a class="nav-item" href="#">Endorsement</a>
        <a class="nav-item" href="#">Contacts</a>
    </div>
</nav>
<main>
    <div class="separator"></div>
</main>


<style>
    nav {
        position: sticky;
        top: -100px;
        width: 100%;
        height: 140px;
        margin-top: -140px;
    }

    nav > div {
        padding-top: 10px;
        padding-bottom: 10px;
    }

    .topside {
        height: 80px;
        display: flex;
        justify-content: center;
        flex-direction: column;
    }

    .botside {
        height: 20px;
        display: flex;
        justify-content: center;
        align-items: center;
        background-color: white;
    }

    .nav-item {
        margin-left: 50px;
        margin-right: 50px;
        text-decoration: none;
        color: rgb(53, 19, 108);
    }

    .separator {
        height: 500vh;
        background-color: red;
    }

    h1 {
        text-align: center;
        margin: 0;
        text-transform: uppercase;
        font-size: xx-large;
        text-shadow: 2px 2px 5px black;
        color: white;
    }

    ul {
        list-style: none;
    }
</style>