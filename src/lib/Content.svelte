<script>
    import Intro from "./Intro.svelte";
    import Creations from "./Creations.svelte";
</script>
<main>
    <Intro />
    <Creations />
</main>
<style>
    main {        
        padding-inline: var(--size-5);
    }

    @media screen and (min-width: 1440px) {
        main {
            padding-inline: var(--size-12);
        }
    }    
</style>