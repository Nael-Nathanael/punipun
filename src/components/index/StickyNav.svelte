<script>
    import {onMount} from "svelte";

    let y;
    let threshold = 1000;

    onMount(() => {
        threshold = vhToPixels(100)
        console.log(threshold)
    })

    function vhToPixels(vh) {
        return Math.round(window.innerHeight / (100 / vh)) - 100;
    }
</script>

<svelte:window bind:scrollY={y}/>

<nav class="w-100 position-sticky d-flex flex-wrap justify-content-center align-items-center bg-light {y > threshold ? 'threshold-reach' : ''}">
    <a href="/">Home</a>
    <a href="#">Shop</a>
    <a href="#">Events</a>
    <a href="#">Games & Equipments</a>
    <a href="#">Endorsement</a>
    <a href="#">Contacts</a>
</nav>

<style>
    nav {
        transition: all .25s ease-in-out;
        transform: translateY(-100%);
        min-height: 40px;
        top: 0;
        z-index: 2000;
    }

    nav.threshold-reach {
        transform: unset;
    }

    a {
        text-decoration: none;
        margin: 2px 20px;
        color: rgb(53, 19, 108);
        display: block;
        font-size: 13px;
    }
</style>