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
        position: relative;        
        /* border: 1px solid lime; */
        --home-height-size: calc(650 / var(--pixels-base) * 1rem);
        width: 100%;
        min-height: var(--home-height-size);        
        padding-inline: var(--size-5);
        padding-block: var(--size-6);
        background-color: hsl(var(--very-dark-gray));
        background-image: var(--hero-mobile);
        background-size: cover;
        background-repeat: no-repeat;
    }

</style>