<script>
    import Logo from "./Logo.svelte";
    import Navbar from "./Navbar.svelte";
</script>
<header class="header">
    <Logo />
    <Navbar />
</header>
<style>
    .header {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }
</style>
