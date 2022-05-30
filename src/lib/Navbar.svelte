<script>
    import NavMobileMenu from './NavMobileMenu.svelte';
    import NavDesktopMenu from './NavDesktopMenu.svelte';
    
    export let isOpen;
    export let isLarge;    
</script>
{#if isOpen && !isLarge}
<div class="mobile-nav-container" >
    <NavMobileMenu />
</div>
{:else}
    {#if isLarge}
    <div class="desktop-nav-container" >
        <NavDesktopMenu />
    </div>
    {/if}
{/if}
<style>
  /* div {
      border: 1px solid red;
  }
    */

 
</style>


  
  
  