<script>
    export let componentLocation;    
    let isFooter;
    let isMobile;
    let isDesktop;

    componentLocation === 'footer' ? isFooter = true : isFooter = false;
    componentLocation === 'mobile' ? isMobile = true : isMobile = false;
    componentLocation === 'desktop' ? isDesktop = true : isDesktop = false;
</script>

<ul class="menu-links" class:footer-menu={isFooter} class:mobile-menu={isMobile} class:desktop-menu={isDesktop}>
    <li><a href="/">About</a></li>
    <li><a href="/">Careers</a></li>
    <li><a href="/">Events</a></li>
    <li><a href="/">Products</a></li>
    <li><a href="/">Support</a></li>       
</ul>

<style>
    li {
       position: relative;
       font-family: 'Josefin Sans', sans-serif;
       margin-left: 1rem;
       font-size: 150%;
       font-weight: 300;
       line-height: var(--font-lineheight-5);        
    }    

    .footer-menu {
        display: flex;
        flex-direction: column;
        justify-content: space-between;
        height: calc(180 / var(--pixels-base) * 1rem);
        font-size: var(--font-size-custom);
    }

    .mobile-menu {        
        margin-top: calc(205 / var(--pixels-base) * 1rem);       
    }

    .desktop-menu {       
        display: flex;       
    }

    @media screen and (min-width: 1024px) {
        li {
            font-size: var(--font-size-custom);
            font-weight: 400;
            margin-left: var(--size-4);
        }

        li::after {
        content: '';
        position: absolute;
        bottom: -0.25rem;
        left: 50%;
        transform: translateX(-50%) scaleX(0);
        height: 2px;
        width: 50%;        
        background: hsl(var(--default-white));
        transition: transform .4s ease-in-out;
        transform-origin: left;
    }

    li:hover::after {
        transform: translateX(-50%) scaleX(1);
    }

        .footer-menu {            
            flex-direction: row;
            height: initial;            
        }

        .footer-menu li {
            margin-left: 0;
        }
    }   
</style>