<script>
    import HeaderBanner from "../components/index/HeaderBanner.svelte";
    import StickyNav from "../components/index/StickyNav.svelte";
    import NewestVideoAndMusic from "../components/index/NewestVideoAndMusic.svelte";
    import FullProfile from "../components/index/FullProfile.svelte";
</script>

<svelte:head>
    <title>Clarissa Punipun Fan Website</title>
</svelte:head>

<HeaderBanner/>
<StickyNav/>

<main>
    <NewestVideoAndMusic/>
    <FullProfile />
</main>

<style>
    main {
        padding: 20px;
        background-color: rgb(53, 19, 108);
    }
</style>