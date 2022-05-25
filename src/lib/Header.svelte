<script>
    import Logo from "./Logo.svelte";
    import MenuBtn from "./MenuBtn.svelte";
    import Navbar from "./Navbar.svelte";

    $: isOpen = false;

    const toggleMenu = () => {
        console.log('toggled');
        isOpen = !isOpen;
    }
</script>
<header class="header">
    <Logo />
    <Navbar {isOpen}/>
    <MenuBtn {isOpen} on:menu={toggleMenu}/>
</header>
<style>
    .header {              
        /* border: 1px solid blue; */
        /* position: relative; */
        margin-top: 0.5rem;
        display: flex;
        justify-content: space-between;
        align-items: center;        
    }
</style>
