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

<main class="pt-0 pb-2 container">
    <NewestVideoAndMusic/>
    <FullProfile />
</main>
