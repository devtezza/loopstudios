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
    /* .navbar {
        border: 1px solid lime;
    } */

    .navbar {        
        position: absolute;
        top: 0;
        left: 0;
        z-index: 2;
        height: 100vh;
        width: 100vw;         
        /* border: 1px solid gold; */
        background-color: hsl(var(--default-black));text-transform: uppercase;
                 

    }  

   /* @media screen and (min-width: 1024px) {
       .navbar {
           z-index: initial;
       }
   } */
</style>
