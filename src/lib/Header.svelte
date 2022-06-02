<script>
    import Logo from "./Logo.svelte";
    import MenuBtn from "./MenuBtn.svelte";
    import Navbar from "./Navbar.svelte";

    const large = '(min-width: 1024px)';
    let componentLocation = 'header';

    $: isOpen = false;
    $: isLarge = matchesQuery(large);

    const toggleMenu = () => {        
        isOpen = !isOpen;
        document.body.classList[isOpen ? 'add' : 'remove']('no-scroll');
    }

    const matchesQuery = (query) => {
        return window.matchMedia(query).matches;
    }    

    const handleResize = (e) => {
        isLarge = matchesQuery(large);
        if (isLarge && isOpen) {
            toggleMenu();
        }
    }    
</script>

<svelte:window on:resize={handleResize}/>

<header class="header">
    <Logo {componentLocation} />
    <Navbar {isOpen} {isLarge}/>
    {#if !isLarge}
    <MenuBtn {isOpen} {isLarge} on:menu={toggleMenu}/>
    {/if}
</header>
<style>
    .header {                     
        margin-top: 0.5rem;
        display: flex;
        justify-content: space-between;
        align-items: center;        
    }
</style>
