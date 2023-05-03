Download Link: https://assignmentchef.com/product/solved-cs2261-lab9-complex-movement-collision-maps
<br>
In this lab, you will be completing several different TODOs, which will, piece by piece, add complex sprite movement. Your code may not compile until you complete an entire TODO block, at which point the game should compile with a new component of the final outcome

(unless otherwise specified).

<h2>TODO 1 – Complex Camera Movement</h2>

We want our jigglypuff to walk only on the screen, and have the camera  follow it without showing something outside of the world.

<ul>

 <li>TODO 1.0</li>

</ul>

CS 2261 Spring 2021

○ In  game.c,  in  the  updatePlayer()  function,  add  in  the  sprite  and  camera movement.

<ul>

 <li>TODO 1.1</li>

</ul>

○ In game.c in the drawPlayer() function, set jigglypuff’s <em>screen </em>row and column in the shadowOAM

■ Hint: the screen row is the world row minus the background vertical offset; the screen col is the world col minus the background horizontal

offset

Your jigglypuff should now be able to walk around and see the entire map, but not off of the edge. The jigglypuff should always be in the middle of the screen unless at the edge of the map (see the example.gba).

<h2>TODO 2.0 – Collision Map</h2>

Now we want our jigglypuff to treat the visuals of the map as if they were actual barriers to movement.

<ul>

 <li>TODO 2.0

  <ul>

   <li>The collision map has been created for you. Open collisionmap.bmp in Usenti and export it. Remember that we want to check the colors of each pixel, so take that into account when choosing export settings. As such, export the collision map as bitmap(GBA) and select 16 bpp. Uncheck the Pal box. TODO 2.1</li>

  </ul></li>

</ul>

○ Include collisionmap.h in game.c.

<ul>

 <li>TODO 2.2

  <ul>

   <li>Update your movement code to only allow jigglypuff to move if the collision map allows it (is white) in the areas that you need to check. Your jigglypuff should not be able to walk over the fences, trees, bushes, and flowers.</li>

  </ul></li>

</ul>

<strong>You will know if it runs correctly if you:</strong>

<ul>

 <li>Your Project.gba has the  same  behavior as  the Example.gba  provided  for  The Example.gba jigglypuff is purple, but Project.gba jigglypuff should be pink.</li>

</ul>

<h1>Tips</h1>

<ul>

 <li>Review recitation materials: Canvas &gt; Recitation Materials</li>

</ul>

○ Complex movement

○ Collision maps