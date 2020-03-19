---
layout: post
title: "Respawning"
date: 2020-03-16
---
Currently in the game, respawning works by selecting the first planet from a list and placing you a set distance from the centre in a random direction. This can cause issues by either dropping you too far away from small planets, that another ends up pulling you in, or worse, spawning you inside the planet due to the hills going further than the distance. My first attempt at fixing this is by casting a ray from the centre of the planet and seeing when it collides with the land, unfortunately this fails due to the collider facing outwards rather than inwards. So next I tried choosing a random point twice the size of the planet away and casting a ray back towards the centre, this gets me the height on the land, where I can then spawn the player. To this I add a small distance in the direction away from the planet in order to stop the player clipping through the ground.
Next I wanted to tackle the planet selection issue, this was a simple fix, rather than picking the first planet found with a 'planet' tag, I just selected a random planet out of the list of planets.
Lastly I want to stop the player from spawning in water. Since all the water only spawns below surface level, when I cast a ray to find land, I can check to see if it is greater than the planet radius away and if not, just reselect a random point. I can see this potentially forcing the game to freeze if the planet selected is mostly water and will have to think of alternatives later.
