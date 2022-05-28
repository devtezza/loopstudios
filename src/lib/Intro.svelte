<section class="intro">
    <div class="intro-image"></div>
    <div class="intro-text">
        <h2>The Leader In Interactive VR</h2>
        <p>Founded in 2011, Loopstudios has been producing world-class virtual reality 
            projects for some of the best companies around the globe. Our award-winning 
            creations have transformed businesses through digital experiences that bind 
            to their brand.</p>
    </div>
</section>

<style>
    .intro {
        padding-top: calc(100 / var(--pixels-base) * 1rem);
        padding-bottom: calc(90 / var(--pixels-base) * 1rem);
        /* padding-top: calc(100 / var(--pixels-base) * 1rem);
        padding-bottom: calc(35 / var(--pixels-base) * 1rem); */
        /* border: 1px solid gold; */
        /* display: grid;
        grid-template-rows: 1fr 1fr; */
        /* gap: var(--size-1); */
    }    

    .intro-image {
        /* border: 1px solid lime; */
        /* height: var(--size-fluid-8);         */
        width: 100%;
        min-height: calc(225 / var(--pixels-base) * 1rem);      
        background-image: url(/images/mobile/image-interactive.jpg);
        background-size: 100%;
        background-position: top center;
        background-repeat: no-repeat;
        /* object-fit: cover; */
    }
   

    .intro-text {       
       text-align: center;
        margin-top: calc(40 / var(--pixels-base) * 1rem);
       /* border: 1px solid pink;    */
    }

   .intro-text p {
        width: 90%;
        /* margin-top: var(--size-3); */
        margin-inline: auto;
        color: hsl(var(--dark-gray));
        font-family: 'Alata', sans-serif;
        font-size: var(--font-size-custom);
        line-height: var(--font-lineheight-4);
        /* border: 1px solid green; */
   }

   @media screen and (min-width: 480px) {
       .intro-image {           
           min-height: var(--size-fluid-10);
       }

       .intro-text p {
           width: 70%;
       }
   }

  
</style>
