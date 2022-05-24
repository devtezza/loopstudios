<script>
    import Hamburger from "./Hamburger.svelte";
    import { createEventDispatcher } from 'svelte';

    const dispatch = createEventDispatcher();

    const eventMenu = () => {
        dispatch('menu')
    };
    
</script>
<button class="menu-btn" on:click={eventMenu}>
    <span>
        <Hamburger />
    </span>
</button>
<style>
    .menu-btn {
        background: none;
        border: none;
    }
</style>
