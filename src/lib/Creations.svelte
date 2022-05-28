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
        <div class="gallery-item" id="grid">
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
        /* border: 1px solid red; */
        /* padding-bottom: var(--size-10); */
        padding-bottom: calc(100 / var(--pixels-base) * 1rem);
    }
    .gallery {
        padding-top: var(--size-5);
        padding-bottom: var(--size-7);
        display: grid;
        gap: calc(23 / var(--pixels-base) * 1rem);
        /* align-items: center; */
        /* border: 1px solid green; */
    }
    .gallery-item {
        /* border: 1px solid red; */
        position: relative;
        /* height: var(--size-11); */
        height: calc(122 / var(--pixels-base) * 1rem);
        width: 100%;
        display: flex;
        align-items: center;
        z-index: 1;
    }
    .gallery-item h3 {
        width: 40%;
        text-align: left;
        margin-top: 2rem;
        margin-left: 2rem;
    }
    .gallery-item:nth-child(4) h3 {
        width: 30%;
    }
    .gallery-item::before {
        content: '';
        position: absolute;
        width: 100%;
        height: 100%;
        background: hsl(var(--default-black) / 0.25);
        /* background: transparent; */
        /* opacity: 0.1; */
        z-index: -1;
    }
    #deep-earth {
        background-image: url(/images/mobile/image-deep-earth.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #night-arcade {
        background-image: url(/images/mobile/image-night-arcade.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #soccer-team {
        background-image: url(/images/mobile/image-soccer-team.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #grid {
        background-image: url(/images/mobile/image-grid.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #from-above {
        background-image: url(/images/mobile/image-from-above.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #pocket-borealis {
        background-image: url(/images/mobile/image-pocket-borealis.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #curiosity {
        background-image: url(/images/mobile/image-curiosity.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    #fisheye {
        background-image: url(/images/mobile/image-fisheye.jpg);
        background-repeat: no-repeat;
        background-size: cover;
    }
    .cta {
        text-transform: uppercase;
        background: none;
        font-family: 'Alata', sans-serif;
        font-weight: 400;
        letter-spacing: var(--font-letterspacing-4);
        font-size: var(--font-size-custom);
        border: 2px solid hsl(var(--very-dark-gray));
        padding-block: calc(9 / var(--pixels-base) * 1rem);
        padding-inline: calc(45 / var(--pixels-base) * 1rem);
        /* margin-inline: auto; */
    }

    @media screen and (min-width: 480px) {
        .gallery-item {
            min-height: var(--size-fluid-9);
        }
   }
</style>