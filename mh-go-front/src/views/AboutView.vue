<template>
  <div class="about">
    <h1>About</h1>
    <hr/>
    <p>Hey there,<br>
     thank you for trying out the Gear Optimizer!<br>
     I hope you can get some use out of this project.
     If you find any bugs, problems, or have some ideas about how to make this site better,<br>
     please let me know via <a rel="stylesheet" href="mailto: pawcessor@gmail.com" target="_blank">pawcessor@gmail.com</a>. Any kind of feedback is welcome, really.<br>
    <br>
     This website kinda grew out of an idea I had, when I was first learning how to code in 2020,<br>
     Back then, I wrote a small algorithm for setting decorations that displayed its results in the console. 
     With that in mind, please be patient with updates to this site, as i can't guarantee that progress will be fast 'n steady,<br>
     but I'd love to keep working on expanding the builder to support further titles of the Monster Hunter Series and features,
     if there is some interest. <br> 
     For more details on what I'm playing around with atm, have a look at the "roadmap" section further down. <br>
     
     Thanks again for stopping by, and have a blast hunting! <br><br>
     Sincerely, <br> Dominik
     
    </p>
  </div>
  <div class="roadmap">
    <hr>
    <h2>roadmap</h2>
    <hr>
    <p>The next steps of development i'd have in mind are these:
      <ul>
        <li>Adding user registration, so you can save your talisman and wishlist configurations.</li>
        <li>Make the page more intuitive, especially on mobile devices.<br>
          Therefore I'd like to overhaul some of the styling and add animations to make expanding/shrinking dropdowns less confusing.</li>
        <li>Expand the Database, so i can make builders for other titles, beginning with Iceborn.</li>
        <li>Afterwards I would love to add a sidebar to navigate builers for different titles.</li>
        <li>Upgrade cat animations in the loading screen.</li>
        <li>More puns.</li>
      </ul>
    </p>
  </div>
  <div class="toolsUsed">
    <h2>Tools Used</h2>
    <p>For everyone interested in the technical aspects of this project, I thought, I'd share some information about the building process. <br>
      First up, this app was created with the MEVN stack and is currently deployed on Heroku. <br>
      The majority of the stack was set up in a pretty standard way, following popular guides on <a href="medium.com" target="_blank">Medium</a>, <a href="https://fireship.io/">Fireship</a>, and StackOverflow for the more finicky parts. <br>

      Regarding the design, these are some of the packages I used in the frontend:
        <ul>
          <li> <a href="https://github.com/sagalbot/vue-select" target="_blank">Vue Select by Jeff Sagal</a></li>
          <li><a href="https://github.com/dafcoe/vue-collapsible-panel" target="_blank">Vue-Collapsible-Panel by dafcoe</a></li>
          <li><a href="https://www.npmjs.com/package/vue-slider-component" target="_blank">Vue-Slider-Component by NightCatSama</a></li>
          <li><a href="https://github.com/shkilo/vue3-draggable">Vue 3 Draggable by Shkilo</a></li>
        </ul>
    </p>
    <p>
      The font I used for most of the UI elements is called<a href="http://www.iconian.com/about.html" target="_blank">"Monster Hunter"</a>  <br>
      If you have any questions concerning details of the setup, or are interested in working together, you're also welcome to contact me via <a rel="stylesheet" href="mailto: pawcessor@gmail.com" target="_blank">Mail</a>. <br>
    </p>
  </div>
  
</template>

<style scoped>
  .about{
    width: 95%;
    max-width: 80em;
    align-self: center;
    border: 3px solid var(--mh-dark-yellow);
    border-radius: 1%;
    padding: 10px  10px 10px 10px;
    margin: 10px 0 10px 0;
    text-align: left;
    background: linear-gradient(180deg, rgba(9,25,55,1) 0%, rgba(19,48,90,1) 100%);
  }
  .roadmap{
    width: 95%;
    max-width: 80em;
    align-self: center;
    border: 3px solid var(--mh-dark-yellow);
    border-radius: 1%;
    padding: 10px  10px 10px 10px;
    margin: 10px 0 10px 0;
    text-align: left;
    background: linear-gradient(var(--mh-dark-green),var(--mh-green));
  }
  .toolsUsed{
    width: 95%;
    max-width: 80em;
    align-self: center;
    border: 3px solid var(--mh-dark-yellow);
    border-radius: 1%;
    padding: 10px  10px 10px 10px;
    margin: 10px 0 10px 0;
    text-align: left;
    background: linear-gradient(var(--mh-dark-red),var(--mh-red));
  }
  .about > p{
    font-family: sans-serif;
    padding: 0 1em 1em 1em;
  }
  .roadmap > p{
    font-family: sans-serif;
    padding: 0 1em 1em 1em;    
  }
  .toolsUsed > p{
    font-family: sans-serif;
    padding: 0 1em 1em 1em;    
  }
  li {
    font-family: sans-serif;
    padding: 0 1em 1em 1em;   
  }
  ul {
    display: block;
    list-style-type: square;
    padding-left: 2em;
  }
  a{
    color: var(--mh-orange);
  }
</style>
