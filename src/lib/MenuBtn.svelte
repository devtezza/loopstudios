<script>
    export let isOpen;
    export let isLarge;
    import Hamburger from "./Hamburger.svelte";
    import Close from "./Close.svelte";
    import { createEventDispatcher } from 'svelte';    

    const dispatch = createEventDispatcher();

    const eventMenu = () => {
        dispatch('menu')
    };    
</script>

<button class="menu-btn" class:transition={isOpen} class:return={!isOpen} on:click={eventMenu}>
    <span>
        {#if isOpen}
        <Close {isOpen}/>
        {:else}
            {#if !isLarge}
            <Hamburger {isOpen}/>
            {/if}
        {/if}
        
    </span>
</button>

<style>
    .menu-btn {
        cursor: pointer;
        z-index: 3;
        background: none;
        border: none;        
    }
    
    .menu-btn.transition {
        animation: var(--animation-scale-up) reverse,  var(--animation-fade-out) reverse;
        animation-duration: .5s;
    }

    .menu-btn.return {
        animation: 
    var(--animation-scale-down) reverse,
    var(--animation-fade-in) reverse;
    animation-duration: .5s;
    }
</style>