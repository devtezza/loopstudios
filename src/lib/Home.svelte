<script>
    import Header from "./Header.svelte";
    import Hero from "./Hero.svelte";
</script>

<div class="home">
    <Header />
    <Hero />
</div>

<style>
    .home {        
        /* border: 1px solid lime; */
        --home-height-size: calc(650 / var(--pixels-base) * 1rem);
        width: 100%;
        min-height: var(--home-height-size);        
        padding-inline: var(--size-5);
        padding-block: var(--size-6);
        background-color: hsl(var(--default-black));
        background-image: url(/images/mobile/image-hero.jpg);
        background-size: cover;
        background-repeat: no-repeat;
    }

</style>