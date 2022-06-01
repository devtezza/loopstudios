<div class="social-icons">
    <a href="/"><img src="/images/icon-facebook.svg" alt="facebook"></a>
    <a href="/"><img src="/images/icon-twitter.svg" alt="twitter"></a>
    <a href="/"><img src="/images/icon-pinterest.svg" alt="pinterest"></a>
    <a href="/"><img src="/images/icon-instagram.svg" alt="instagram"></a>
</div>

<style>
    .social-icons {
        display: grid;
        grid-template-columns: repeat(4, 1fr);
        justify-items: end;
        align-items: end;        
        padding-block: var(--size-5);
        padding-inline: 30%;        
    }

    .social-icons a {
        position: relative;
        /* border: 1px solid red;         */
    }

    .social-icons a::after {
       position: absolute;
       content: '' ;
       width: 100%;
       height: 2px;
       background: hsl(var(--default-white));
       bottom: -0.75rem;
       left: 0;
       transform: scaleX(0);
       transition: transform .3s ease-in;
       transform-origin: left;
    }

    .social-icons a:hover::after {
        transform: scaleX(1);
    }

    @media screen and (min-width: 500px) {
        .social-icons {
            padding-inline: 35%;
        }
    }

    @media screen and (min-width: 768px) {
        .social-icons {
            padding-inline: 40%;
        }
    }

    @media screen and (min-width: 1024px) {
        .social-icons {           
            grid-area: social;           
            padding: 0;
            padding-left: 100px;
            /* border: 1px solid red; */
        }
    }
</style>