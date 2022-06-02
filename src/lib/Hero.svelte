<div class="hero">
    <div class="h1-frame">
        <h1 class="h1">Immersive Experiences That Deliver</h1>
    </div>    
</div>

<style>
    .hero {
        margin-top: var(--size-12);
        color: hsl(var(--default-white));        
    }

    .h1-frame {
        width: 100%;
        border: var(--border-size-2) solid;
        padding: var(--size-4);
    }

    @media screen and (min-width: 768px) {
        .h1-frame {
            width: 50%;
        }
    }

   @media screen and (min-width: 1440px) {
       .hero {
           margin-top: var(--size-11);
       }

       .h1-frame {
            width: calc(675 / var(--pixels-base) * 1rem);            
            padding: 2.5rem;
       }
   }
</style>