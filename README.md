# roadmap-anims
just some notes idk

<span style="color: red;">This text is red or whatever, trying out css inline stuff.</span>

Here's a cool tutorial to create dynamic face that can be applied into our animation using Moon Animator.
1. Open 3d Paint (the software I use, but anyone can switch to a better alternative such as Photoshop) and then apply 420 x 420 canvas size. Don't forget to uncheck the "Lock Aspect Ratio" and "Resize with canvas" checkbox.
2. Draw the face as you please but don't draw the pupils, then export it as a png file to your folder.
3. Open your Roblox Studio, create a blank Part (name it 'Face' for convenient sake) and add the decal object. Within that decal's property, find the 'ColorMapContent' property so we can import the face we just made earlier.
4. Now moving on to making the pupils. The reason why we're doing this NOW in Roblox Studio is so we can control the eye movement using Moon Animator's keyframe, something like that. Create a cylinder part, recolor, resize, whatever you require until it fits as your characters pupils. Make a duplicate of it and change both parts name into something that you can remember easily. Make sure to put both pupil parts inside of your Face part. 
5. Use the EasyWeld plugin to append your pupils part and attach it to the face part. Afterwards set the face's part transparency to 0.
6. Import your characters rig and delete the face decal, if it didn't work out as intended then search for faceless head in the Toolbox, grab the SpecialMesh object and replace the Mesh object on your characters head rig. Don't forget to put the Face part to your characters head rig folder as well.
7. Grab your Face part and position it to the rigs head (front-face) accordingly, then finally we use EasyWeld plugin to append the newly face part as a replacement for our faceless characters rig. (Animatable should be checked)
