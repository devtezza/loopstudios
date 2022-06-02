<section class="creations">
    <h2>Our Creations</h2>
    <div class="gallery">
        <div class="gallery-item" id="deep-earth">
            <h3>Deep Earth</h3>
        </div>
        <div class="gallery-item" id="night-arcade">
            <h3>Night Arcade</h3>
        </div>
        <div class="gallery-item" id="soccer-team">
            <h3>Soccer Team VR</h3>
        </div>
        <div class="gallery-item" id="the-grid">
            <h3>The Grid</h3>
        </div>
        <div class="gallery-item" id="from-above">
            <h3>From Up Above VR</h3>
        </div>
        <div class="gallery-item" id="pocket-borealis">
            <h3>Pocket Borealis</h3>
        </div>
        <div class="gallery-item" id="curiosity">
            <h3>The Curiosity</h3>
        </div>
        <div class="gallery-item" id="fisheye">
            <h3>Make It Fisheye</h3>
        </div>
    </div>
    <button class="cta">See All</button>
</section>
<style>
    .creations {
        text-align: center;        
        padding-bottom: calc(100 / var(--pixels-base) * 1rem);
    }
    
    .gallery {
        padding-top: var(--size-5);
        padding-bottom: var(--size-7);
        display: grid;
        gap: calc(23 / var(--pixels-base) * 1rem);       
    }

    .gallery-item {       
        position: relative;        
        height: calc(122 / var(--pixels-base) * 1rem);
        width: 100%;
        display: flex;
        align-items: center;
        z-index: 1;
        background-repeat: no-repeat;
        background-size: cover;
        cursor: pointer;
    }

    .gallery-item h3 {
        width: 40%;
        text-align: left;
        margin-top: 2rem;
        margin-left: 2rem;
        transition: all .4s ease-in;
    }

    .gallery-item:nth-child(4) h3 {
        width: 30%;        
    }

    .gallery-item::before, .gallery-item::after {
        content: '';
        position: absolute;
        width: 100%;
        height: 100%;    
        z-index: -1;
    }

    .gallery-item::before {
        background: hsl(var(--default-black) / 0.25);
    }

    .gallery-item::after {
        background: hsl(var(--default-white) / 0.75);
        transform: scaleY(0);
        transition: transform .4s ease-in-out;
        transform-origin: bottom;
    }

    .gallery-item:hover h3 {
        color: black;
    }

    .gallery-item:hover::after {
        transform: scaleY(1);
    }   

    #deep-earth {
        background-image: var(--deep-earth-mobile);
        
    }

    #night-arcade {
        background-image: var(--night-arcade-mobile);
        
    }

    #soccer-team {
        background-image: var(--soccer-team-mobile);
       
    }

    #the-grid {
        background-image: var(--the-grid-mobile);
       
    }

    #from-above {
        background-image: var(--from-above-mobile);
       
    }

    #pocket-borealis {
        background-image: var(--pocket-borealis-mobile);
       
    }

    #curiosity {
        background-image: var(--curiosity-mobile);      
    }

    #fisheye {
        background-image: var(--fisheye-mobile);        
    }

    .cta {
        position: relative;
        text-transform: uppercase;
        background: none;
        border: none;
        font-family: 'Alata', sans-serif;
        font-weight: 400;
        letter-spacing: var(--font-letterspacing-4);
        font-size: var(--font-size-custom);
        border: 2px solid hsl(var(--very-dark-gray));       
        padding-block: calc(9 / var(--pixels-base) * 1rem);
        padding-inline: calc(45 / var(--pixels-base) * 1rem);
        cursor: pointer;
        transition: all .3s ease-in;
        z-index: 1;
    }

    .cta::after {
        position: absolute;
        content: '';
        width: 100%;
        height: 100%;
        top: 0;
        left: 0;
        background: hsl(var(--default-black));        
        border: 2px solid hsl(var(--default-black));
        border: none;
        transform: scaleX(0);
        z-index: -1;
        transform-origin: left;
        transition: transform .3s ease-in;
    }    

    .cta:hover {        
        color: hsl(var(--default-white));
        border: 2px solid hsl(var(--default-black));        
    }

    .cta:hover::after {
        transform: scaleX(1);
    }

    @media screen and (min-width: 480px) {
        .gallery-item {
            height: var(--size-fluid-9);
        }
    }

    @media screen and (min-width: 768px) {
        .gallery {
            grid-template-columns: 1fr 1fr; 
        }

        .gallery-item {           
            height: var(--size-fluid-8);
        }       
    }

    @media screen and (min-width: 1024px) {
        .creations {
            display: grid;
            grid-template-areas:
             "creations-h2 2fr cta"
             "gallery gallery gallery";
        }

        .creations h2 {
            grid-area: creations-h2;
        }

        .gallery {
            grid-template-columns: repeat(4, 1fr);
            grid-area: gallery;
        }

        .gallery-item {
            align-items: flex-end;            
            height: 28rem;
            background-position: left top;
            background-size: cover;
        }

        .gallery-item h3 {
            width: 50%;
            font-size: 200%;
            margin-bottom: var(--size-7);            
        }       

        .gallery-item:nth-child(3) h3 {
            width: 65%;        
        }

        .gallery-item:nth-child(3n+5) h3 {
            width: 75%;        
        }

        #deep-earth {
        background-image: var(--deep-earth-desktop);        
        }

        #night-arcade {
            background-image: var(--night-arcade-desktop);
        }

        #soccer-team {
            background-image: var(--soccer-team-desktop);
        }

        #the-grid {
            background-image: var(--the-grid-desktop);        
        }

        #from-above {
            background-image: var(--from-above-desktop);
        }

        #pocket-borealis {
            background-image: var(--pocket-borealis-desktop);
        }

        #curiosity {
            background-image: var(--curiosity-desktop);      
        }

        #fisheye {
            background-image: var(--fisheye-desktop);        
        }

        .cta {
            grid-area: cta;
        }        
    }

    @media screen and (min-width: 1440px) {
        .gallery {
           padding-top: var(--size-9);
           padding-bottom: var(--size-10); 
           gap: var(--size-7);
        }

        .cta {
           height: 70%;
        }        
    }
</style>