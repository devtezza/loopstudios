<script>
    import { slide } from 'svelte/transition';
    export let isOpen;
</script>
{#if isOpen}
<nav class="navbar" transition:slide>
    <ul class="navbar-menu">
        <li><a href="/">About</a></li>
        <li><a href="/">Careers</a></li>
        <li><a href="/">Events</a></li>
        <li><a href="/">Products</a></li>
        <li><a href="/">Support</a></li>      
    </ul>    
</nav>
{/if}
<style>
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

   .navbar-menu {        
        margin-top: calc(205 / var(--pixels-base) * 1rem);       
   }

   li {
       font-family: 'Josefin Sans', sans-serif;
       margin-left: 1rem;
       font-size: 150%;
       font-weight: 300;
       line-height: var(--font-lineheight-5);        
   }
</style>


  
  
  