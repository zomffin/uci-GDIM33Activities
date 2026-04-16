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
