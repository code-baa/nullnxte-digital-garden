---
{"dg-publish":true,"dg-path":"devlogs/prologue.md","permalink":"/devlogs/prologue/","dgHomeLink":true,"dgShowBacklinks":true,"dgShowInlineTitle":true,"dgShowFileTree":true,"dgEnableSearch":true,"dgShowToc":true,"dgLinkPreview":true,"dgShowTags":true,"noteIcon":""}
---

---
<a href="/" target="_self">← Go back home</a>
 
### Prologue: The road here

>
  *We did this not because it was easy, but because we thought it would be easy.*
> 
 
 
 
 
Making games is hard. 

Any single discipline in game development is a potential career path to pursue. And making a game 'solo' means you have a lot of things you need to be 'okay enough' at. Something I've learned is that approaching any large task without giving up is just a matter of rowing your boat toward the horizon knowing that you may never 'get' there -- you just have to make yourself enjoy rowing. 

In game development you're a designer, a programmer, an animator, a modeler, a composer, a sound designer, a UI designer -- and I'm afraid that is just the tip of the iceberg. 

It really comes as little surprise when a person interested in getting started might see this monumental workload and promptly decides to pull the ripcord. I've dropped and picked up 'game dev' too many times to count. The wasteland of unfinished projects on my hard drives are a testament to that journey: tech demos, environmental demos, random little simulations -- they pepper my project folders like the barnacles on a boat heading nowhere. 

But as these interests ebb and flow, you pick up a little something from each of them. My first foray into 'game development' was making maps in Hammer for CounterStrike: Source. Soon, I picked up GameMaker 8, where I learned the basics of scripting and pixel-art. Over many years I moved to GameMaker Studio, GameMaker Studio 2, Unity, and finally Godot. 

<div style="
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 5rem;
  gap: 1rem;
">

  <!-- Flywheel card -->
  <div style="
    position: relative;
    width: 100%;
    max-width: 350px;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 6px 15px rgba(0,0,0,0.2);
    transition: transform 0.3s ease;
  " onmouseover="this.style.transform='scale(1.03)'" onmouseout="this.style.transform='scale(1)'">
      <img 
        src="https://github.com/code-baa/nullnxte-digital-garden/blob/main/public/images/fishing.gif?raw=true" 
        alt="Fishing GIF" 
        style="width: 100%; display: block;"
      />
  </div>
  <!-- Description text -->
  <p style="
    width: 100%;
    max-width: 380px;
    margin:0;
    font-size:1rem;
    line-height:1.5;
    text-align: center;
  ">
    Fishing environmental test made in GameMaker Studio, 2015. <br> <br> I won't be winning any awards for pixel-art, but this fishing project from over 10 years ago was my first explorations into game design. I opted for a horizontal fishing meter so that the back-and-forth motion simulated the 'leading' of fish that anglers must do to keep tension on the hook. Stardew Valley would release the next year with a vertical fishing meter much like this design.
  </p>

</div>


<div style="
  display: flex;
  flex-direction: column;
  align-items: center;
  margin-top: 5rem;
  gap: 1rem;
">

  <!-- Flywheel card -->
  <div style="
    position: relative;
    width: 100%;
    max-width: 350px;
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 6px 15px rgba(0,0,0,0.2);
    transition: transform 0.3s ease;
  " onmouseover="this.style.transform='scale(1.03)'" onmouseout="this.style.transform='scale(1)'">
      <img 
        src="https://github.com/code-baa/nullnxte-digital-garden/blob/main/public/images/cell_simulation.gif?raw=true" 
        alt="Cell simulation GIF" 
        style="width: 100%; display: block;"
      />
  </div>
  <!-- Description text -->
  <p style="
    width: 100%;
    max-width: 380px;
    margin:0;
    font-size:1rem;
    line-height:1.5;
    text-align: center;
  ">
    Cell simulation made in GameMaker Studio, 2018. <br> <br> Cells have a lifespan that increases based on their food intake. Each cell has a genetic string that determines their movements. Once a threshold is reached, the cell reproduces, imparting it's genetic string to an offspirng.
  </p>

</div>
 
 
 
 
 
































<p>
This year I did a game jam and actually finished a game with a full loop and a couple of levels. It's called Flywheel. You slot different pistons into an engine while managing stress levels to ensure it can run consecutively. 
<img style="float:right;" src="https://img.itch.zone/aW1hZ2UvMzQwOTM2MS8yMDM0ODYxOC5wbmc=/347x500/RKkta6.png"/>
</p>










Ever since college I would make environmental, tech, or simulation demos in GameMaker. Before that, I was obsessed with map-making in Hammer & Unreal game SDK's. But my
I started integrating my FPS project into the multiplayer implementation project. i got movement and mouse look working over the weekend.  today i tested it with glock and banther by port forwarding and connecting to my external IP. it worked fantastically. they noted how smooth it was and said the game felt very responsive.

im very happy with the results. it is definitely going to be a challenge to integrate all of what i have into multiplayer, but i have given myself two weeks to do it. tonight i will hopefully get hit scan and the basics of enemies in. 

the plan is to fully port what i have now into multiplayer, and from now on build from that. once i get it ported, i will add steam integration. as far as i know it is as 'simple' (lol) as replacing ENet with steams API. we will see how simple it is in reality. 

i still am not fully comfortable in the multiplayer codebase. it feels very clunky and spaghetti. There are function calls and globals and signals all mixed together. im hoping the longer i spend in the codebase, the clearer it will become. im going to try and build a flowchart that lays the entire thing bare. maybe thats silly and a waste of time, but maybe not and i learn a bit more about how it all fits together. either way im pleased with how ive been adding onto the protobuffers and syncing my own variables across the network; i picked that up quick and it feels great that it works. 