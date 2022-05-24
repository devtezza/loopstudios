<script>
    export let isOpen;
</script>
{#if isOpen}
<nav class="navbar">
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
        /* overflow-y: hidden;
        height: 25px;         */
        border: 1px solid gold;
        /* transform: translateY(-200px); */
    }

   ul {
        justify-content: space-between;
   }

   /* ul.active {
    
   } */

   li {
       margin-left: 1rem;
   }
</style>


  
  
  