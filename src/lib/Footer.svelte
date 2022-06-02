<script>
  import Logo from './Logo.svelte';
  import MenuLinks from './MenuLinks.svelte';
  import Social from './Social.svelte';
  let componentLocation = 'footer';
</script>
<footer class="footer">
  <Logo {componentLocation}/>

  <div class="footer-menu-container">
  <MenuLinks {componentLocation}/>
  </div>

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
  
    .footer-menu-container {
        margin-block: var(--size-7);
        text-align: center;
    }   

    .copyright, .attribution {
      font-size: var(--font-size-custom);
        text-align: center;
        color: hsl(var(--dark-gray));
    }

    .attribution {
      grid-area: attribution;       
      font-size: 11px;       
      margin-top: var(--size-3); 
    }
    .attribution a { 
      color: var(--blue-9); 
    }

    @media screen and (min-width: 1024px) {
      footer {
        display: grid;
        /* grid-template-columns: repeat(3, 1fr);
        grid-template-rows: repeat(3, 1fr); */
        grid-template-areas:
          "logo . social"
          "menu-container . copyright"
          ". attribution ."
        ;
        gap: 25px;
        justify-content: space-between;
        align-items: center;
        padding-inline: 25px;
      }
      .footer-menu-container {
        grid-area: menu-container;
        margin: 0;
        width: var(--size-14);
      }
      .copyright {
        grid-area: copyright;
      }
    }

    @media screen and (min-width: 1440px) {
      .footer {
        /* border: 1px solid green; */
        padding-top: 2.5rem;
        padding-inline: var(--size-12);        
      }
      .attribution {
        margin-top: initial;        
      }
    }
</style>