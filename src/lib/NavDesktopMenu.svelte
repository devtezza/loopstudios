<script>
    import { slide } from 'svelte/transition';
    import MenuLinks from "./MenuLinks.svelte";
    let componentLocation = 'desktop';
</script>

<nav class="navbar" transition:slide>
    <MenuLinks {componentLocation} />    
</nav>

<style>
    .navbar {                
        position: initial; 
        background-color: transparent; 
    } 
</style>
 