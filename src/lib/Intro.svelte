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
    }    

    .intro-image {        
        width: 100%;
        min-height: calc(225 / var(--pixels-base) * 1rem);      
        background-image: var(--interactive-mobile);
        background-size: 100%;
        background-position: center top;
        background-repeat: no-repeat;       
    }   

    .intro-text {       
       text-align: center;
       margin-top: calc(40 / var(--pixels-base) * 1rem);       
    }

   .intro-text p {
        width: 90%;        
        margin-inline: auto;
        color: hsl(var(--dark-gray));
        font-family: 'Alata', sans-serif;
        font-size: var(--font-size-custom);
        line-height: var(--font-lineheight-4);        
   }

   @media screen and (min-width: 480px) {
       .intro-image {           
           min-height: var(--size-fluid-10);
       }

       .intro-text p {
           width: 70%;
       }
    }

    @media screen and (min-width: 768px) {
        .intro-image {
            background-image: var(--interactive-desktop);
        }
    }

    @media screen and (min-width: 1024px) {
       .intro {
           display: grid;
           grid-template-columns: repeat(5, 1fr);
           grid-template-rows: repeat(5, 1fr);           
       }

       .intro-image {
           grid-column: 1 / 5;
           grid-row: 1/6;
           height: initial;          
           background-position: right top;
       }

       .intro-text {
           grid-column: 4 / 6;
           grid-row: 3 / 6;
           background-color: hsl(var(--default-white));
           margin: 0;
           padding-top: var(--size-fluid-5);
           padding-left: var(--size-fluid-5);
           text-align: left;
       }

       .intro-text p {
           margin: 0;
           width: 100%;
       }      
    }

    @media screen and (min-width: 1440px) {
        .intro {
            padding-top: calc(150 / var(--pixels-base) * 1rem);            
            grid-template-columns: repeat(6, 1fr);
            grid-template-rows: repeat(6, 1fr);          
        }

        .intro-image {
            grid-column: 1 / 5;
            grid-row: 1/6;
        }

        .intro-text {
            grid-column: 4/ 7;
            grid-row: 3 / 6;
            padding-top: var(--size-10);
            padding-left: var(--size-11);
        }
    }
</style>