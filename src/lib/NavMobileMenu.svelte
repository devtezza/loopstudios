<script>
    import { slide } from 'svelte/transition';
    import MenuLinks from "./MenuLinks.svelte";
    let componentLocation = 'mobile';
</script>

<nav class="navbar" transition:slide>
    <MenuLinks {componentLocation} />
    <div>{componentLocation}</div>
</nav>

<style>   
    .navbar {        
        position: absolute;
        top: 0;
        left: 0;
        z-index: 2;
        height: 100vh;
        width: 100vw;                 
        background-color: hsl(var(--default-black));text-transform: uppercase; 
    }
</style>