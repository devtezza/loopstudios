<script>
  import Logo from './Logo.svelte';
  import FooterMenu from './FooterMenu.svelte';
  import Social from './Social.svelte';
  let logoLocation = 'footer'  ;
</script>
<footer class="footer">
  <Logo {logoLocation}/>

  <FooterMenu />

  <Social />
    <div class="copyright">
        © 2021 Loopstudios. All rights reserved.
    </div>
    
  <div class="attribution">
    Challenge by <a href="https://www.frontendmentor.io?ref=challenge" target="_blank">Frontend Mentor</a>. 
    Coded by <a href="https://www.devtezza.com/">Fernando Tezza</a>.
  </div>
</footer>

<style>
    footer {
      padding-top: var(--size-8);
      background: hsl(var(--default-black));
      color: hsl(var(--default-white));      
    }   

    .copyright, .attribution {
        text-align: center;
        color: hsl(var(--dark-gray));
    }
    .attribution {       
      font-size: 11px; 
      
      margin-top: var(--size-3); 
    }
    .attribution a { 
      color: var(--blue-9); 
    }
</style>