# GDIM 33 In-Class Activities
## W1
### Activity 1
[Inspo Board](https://miro.com/app/board/uXjVGoFLFn0=/?share_link_id=573951097400)


1. I love medieval stuff right now... I also have been playing a lot of action games of various types. And it's not super represented in my moodboard, but I also really love low poly (mid poly...?) games with crunchy textures. 
2. I talked with my other table mates and there was an interesting mix of ideas and aesthetics people are interested in. One person had a very Y2K board and mentioned wanting to do a platformer with nyan cat (awesome). Another person also likes action games like me but is hesitant about how to make it because of how art intensive a game with combat is.
3. I talked with Agnes about games, and she mentioned how she likes RPGs and single player games with mood. Particularly she said her favorite game is Baldur's Gate 3. I also like RPGs, but I have a hard time actually finishing them. I never finished a singleplayer playthrough of Baldur's Gate 3, but I did finish a co-op playthrough- I really liked the combat, but wasn't able to really experience or immerse myself in the story because of the nature of co-op splitting up cutscenes between people. 


### Activity 2
1. Typing game + Papers, Please-like + Resource management
2. A document management game including typing mini-games. Players are asked to do a set of tasks that require resources. Once they finish, they must fight with other NPCs over office resources in a pool (kind of like hungry hungry hippo). They'll have a limited amount of time to grab resources (while also fighting other NPCs for them). Papers, Please-like in the way players will have to manage a bunch of documents, but there won't be NPCs that you're checking/comparing in that way (maybe, this idea is a bit nebulous right now). Kind of like being in hell but its a competitive office workspace. Particularly, I want mistakes to cost resources (ex. if you make a typo and have to delete, it takes up both ink and eraser resources). Creepy/horror aesthetic, kind of like Dead Letter Dept., Buckshot Roulette, or No I'm Not Human. 
   (maybe it'll be JUST the typing game, for scope sake).
4. [Planning drawing](https://docs.google.com/drawings/d/1FEoPs119xbTbxzRwz5_9L2jFhjPmUyWcokSxR4krJ34/edit?usp=sharing)


## W2
activities :)

## W3
### Activity 1
[Updated Planning Drawing](https://docs.google.com/drawings/d/1FEoPs119xbTbxzRwz5_9L2jFhjPmUyWcokSxR4krJ34/edit?usp=sharing)

## Activity 2
1. Saving the event name is advantageous because it'll reduce errors due to typos from needing to retype it several times.
2. I used debug logs to track when the states were changing, and when interaction with the walrus is true/false. This helped me test if the transitions were working correctly (which they weren't at certain steps). Then I added more debug logs tied to the events that were supposed to trigger the events to check if those were firing (they were not). It helped me figure out that I wasn't correctly hooking up the gameobject to the trigger custom event node.
3. Set Cursor Lock State is relevant to my project. Generally the cursor won't be locked (most of the game involves clicking on objects to interact with them), but when they're in the typing minigame, I want to lock it so the player doesnt have to worry about bumping their mouse or something.
4. The concept of a game state is relevant to my vertical slice. It's going to have 2 different modes, the task completion part and the resource collection phase. The game manager will have to spawn and set up things related to both modes, as well as moving the camera and restricting what the player can do in either mode.


## W4
### Activity 1 Playtesting
The main typing minigame is playable right now. Tasks will spawn in, and the player can complete tasks in a set order- once all tasks are "finished" (regardless if they're correct or not), gives out new tasks. 
My playtesting goals is to see if there's any big issues with typing (in terms of accuracy)

#### Playtesting Group
Zoya McDonnell, Kristin Zhang, Andy Nguyen, Jacob Ho

#### Playtesting Notes
- People don't quite understand how to get in and out of the typing mode
- Some passages are probably too long ....
- Also need a way to wrap text or have tasks spawn multiple pages 
- The paper on the "typewriter" is angled so any overflow text disappears\
- Brandon suggestion: maybe split up longer passages into sentences so this game doesnt explode people's ram

### Activity 2
1. Yes, to a degree. It's not too bad to add new nodes and connect them to the existing scriptable objects. An issue may come up if you want a LOT of options because the ui becomes super cramped or bleeds off the screen. 
2. 4 options
3. The regenerate nodes option forces unity to run through the project and read through new scripts or imported libraries for possible nodes. It'll read up new functions that can be turned into nodes.

im too hungry to do this bonus point sorry

## W5
### Activity 1, Steps
Implementing a game over 


**Simple** 

Step 1: Detect game over
Step 2: Pause the game and throw up new UI canvas 
Step 3: Restart implementation 

**Complex** 

Step 1: Typing script triggers an event when ANY resource is down to 0, notifies gamemanager graph. Should have 1 arg for which resource ran out. Test with Debug.Logs.

Step 2: Have the event pause all current activity and throw up a new UI canvas. 

Step 3: Have game over UI show appropriate text

3a: What resource ran out + what was left of other resources

3b: New stat tracking, like tasks completed and overall accuracy

Step 4: Have a button for restarting the game, use Debug.Log to see if it was pressed 

Step 5: Have the button reload the scene 

Step 6: Properly reset all values on reload (Debug.Logs to check) 

### Activity 2
I was able to fully implement a game over screen with a restart button. It shows a unique "you ran out of..." message depending on which resource was depleted, as well as overall stats for all the resources + overall accuracy + completed tasks. 
Next I wanna have the accuracy score reset during different phases of gameplay, so when you return to typing its a clean slate.


## W6
### Activity 1
1. What's new in the game... is the game end and the NPC. Also had some major bugs that probably existed in milestone 1 that are now fixed.
2. [New Link](https://zomffin.itch.io/33-milestone-2)
3. My playtest goal is mainly to see if there's any major bugs with game ending and the NPC.


### Activity 2
1. Multiply makes things darker and less saturated because its multiplying the 2 vectors together, and the values are being multiplied by decimals, so the numbers are getting smaller. As the values approach 0, there's less of each color value, and it approaches black.
2. It will be more transculent. 1 alpha means its opaque, 0 means its completely see through. Like above, the numbers are multiplied to be smaller and smaller, so they're getting more transculent.
3. The shader gets the UV values from the mesh. The vertices in the mesh also store the UV values, so it's just directly taking it.
4. Math is scary.... but colors are cool. Also I'm familiar with blending modes already because of using digital art programs, so I'm very excited to translate some of that knowledge.


## W7
1. The data for the Vertex Color node comes from the mesh.
2. Because the colors are stored on each vertex, then the areas between the vertexes, the polygons, are blended between the vertexes. So if the color from vertex A is tan, and the vertex from B and C are white, then the areas between those would be a mix of tan and white.
3. The textured shiba is more accurate because it's assigning specific color values per the UVs, which accounts for the full polygons. Vertex colors could be good for models that don't need very specific colors, or using the gradients/mixing on purpose.
4. There's something wrong with it's left hindleg, theres roughly a polygon appearing wrong.
5. You could check the UV values on the mesh and see if anything seems obviously displaced or disconnected to surrounding polygons. 
6. It's the error we see in the normal debug shader.
7. When it's alpha, it's not fully transparent but just a darker color. 

## W8
### Playtesting/Activity 1
- There's now some difficulty scaling (you get more tasks as you complete rounds, and at specific rounds other NPCs become active and will compete for resources).
- [New Link](https://zomffin.itch.io/33-milestone-3)
- Playtesting goals is to see if the tutorial helps (haven't seen people play with tutorial), check for any bugs, and see if the difficulty scaling works (and if it breaks anything).

Notes: Tutorial lowkey doesn't work because people don't want to fully read it (and don't understand what the phrase they have to type is). 
- There's a bug with task spawning- they're doubling up when it's not intended
- Texture error with the player "hand"

### Activity 2C
1. It seems like there's a couple passes associated with the post-processing effect. FullScreenPassRendererFeature has the full strength effect, while Finalblit adds the transparency. I can tell because when I go through the passes, the effect first appears with FullScreenPassRendererfeature. As I step through, I can see the effect appear and change to its final form. 
2. Lerp has a transparent version of the fullscreen effect. At 0, the game looks normal, and at 1, it's at full strength (like before we added the lerp).
3. The screen looks like that because Lerp is combining the normal screen with the effect at different percentages. It's like setting the opacity of the effect, as it effects less and less as you approach 0.
4. I checked out the effect with just time(sin), and I noticed it would make the screen more green. I realized this is because sin goes from -1 to 1, so -1 must have an opposite effect on the mixing (since green is the complementary to red?). By using (sin+1)/2, we first take out any instance of -1, and then by dividing it by 2, the range becomes 0 to 1 (the proper 0-100%). 

## W9
### Activity 1
We chose a game called Pyre by Supergiant Games. We were analyzing the dialogue box, anod how it transitions between spoken character dialogue to the narrator/exposition. The effect seems to be a renderer feature applied to specific items. There's a lighter white section of the dialogue box that can fade in and out (it's there for spoken dialogue), but in fades in a way similar to a paper burning (ie. not equal across the texture but instead near the edges and in spots in the middle). It's probably using some sort of texture/noise to guide the parts it starts the fading at, and goes through the grayscale. 

I think it's an animation thats triggered, and also technically a layer on top of the "base" dialogue box. The animation is triggered at transition points in dialogue on click. If this were something like the dialogue nodes we've used in class/in 32, the node itself could have a bool indicating whether or not the node after/before it is a change from dialogue -> exposition or vice versa, and the script can trigger the animation based on it. 

### Activity 2
I didn't work on the shader or it's activation because I already finished that. However, I was having a building bug where the shader wasn't being built for WebGL, so I had to change some project settings to fix that. I also made a small bug fix for how tasks spawn (they were spawning more than once), as well as adding different NPC stats and more resources dropping as new NPCs spawn in. 
