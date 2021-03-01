# My-portfolio
This project was something I created in my game design class. The idea was to create a game in the same style and spirit as the popular video game series Mega Man 
(Mega man 2 specifically). The requirements were that I have at least 2 different weapon types to be able to swap between, 2 enemy types, at least one fully completed 
level to navigate, and a final boss at the end of the level. For those that might not be aware, Mega man is a popular video game franchise that is known as a platformer game. 
Other well known platformer games include the Mario games as well as early Zelda games. While the project isn't an exact replica of the game Mega Man, the goal was to create 
something more in line with the spirit and basic ideas of Mega Man. The software that was used to make the project is called Game Maker 2. It's an excellent tool great for
developing 2D games like this. As a side note: I'm also using this software to develop recreations of games like Pong and Pac Man, which is just to name a few examples of what
Game Maker 2 is capable of producing. As far as the project itself, I'll disect it bit by bit to describe how it was put together as well as how it works. The images and 
characters shown in game are called the sprites. You'll notice that some of them are relatively basic and featureless, while others are much more thought out and well detailed. 
The floor, projectiles, and enemy projectiles are meant to be basic in order to cut down on the visual noise of a project like this and being able to tell things apart from one
another. For example, the enemy projectiles are meant to be different looking compared to yours so that while you're in the middle of playing, everything doesn't seem too 
confusing and threats are easier to identify. The enemy projectiles themselves also move noticably slower compared to the player projectiles, but we'll get into that in a moment.
As far as the more detailed Mega Man sprites as well as the background, these are not my own creations. As part of the project, we were given permission to find assets online to
use as our Mega Man characters and themes. I found a website called Spriters-Resource and used the Mega Man 2 assets provided for my Mega Man character, enemies, boss, and other 
objects. The background was also found doing a quick google search for a pixilated space themed background. The citations for these websites are part of the zip file in a text 
document. The sprites are not what the main focus is of the actual program. They are what makes the game look the way it does, sort of like the icing on the actual cake. The 
objects themselves is where everything begins to interact with each other to make the game function the way it does. The player character Mega Man is known in the code as 
heroObject. We also have objects such as floorObject, enemyObject, stompObject, enemyObject2, projectileObject, enemyProjectileObject, ammoBoxObject, and finally bossObject. All 
of these objects interact with the game's world in many different ways in order to get everything working as it's intended. The most complicated object in the whole program is 
the heroObject, or Mega Man himself. As the player, you are the one who interacts with everything the game has to offer. The movement, the weapons, enemies, projectiles, the 
platforms, the final boss, and the collectable ammo boxes that you'll need to keep your weapons loaded and the enemies at bay. As such, Mega Man has so many various events taking
place. The most commonplace event that is almost constantly taking place is the collision event. As one can guess, collision events is what happens, to Mega Man in this instance,
when he collides or makes contact with certain objects. For instance, if the player were to make direct contact with the an enemy object, Mega Man would take damage and lose one 
of his 3 lives. There is also another collision with our other object called stompObject. The stompObject is directly linked to all enemyObjects and is invisible in game. It's 
function is to destroy itself and it's parent object (in this case enemyObject) when making contact with Mega Man. So if Mega Man makes contact with the enemy in the right spot,
the enemy will be destroyed and Mega Man can make progress. The same also applies when they make contact with Mega Man's projectile attacks. Speaking of projectiles, Mega Man 
has 2 different weapons that he can swap back and fourth to with the push of a button. His primary weapon consists of a basic straight shooting projectile that destroys any enemy 
object that it comes into contact with. The secondary weapon operates the same way but with a twist, the projectiles shoot out in a burst in three seperate directions. Both
weapons shoot in the direction the player is facing. However, each time the weapon is fired the ammo counter gets closer to depleteing and the player is unable to attack.
This is where the ammoBoxObject comes in. When the player collides with these objects, the ammo counter increases by 5. These can also stack up past 10, so collecting an 
abundance of them is worth doing. The boss fight, while not the most creative part, is something that has importnant features worth noting. Despite the fact that he has his 
own burst projectile attack, the boss has a noticable health indicator over his head. The number representing the amount of health points he has. Once his health meter gets 
down to zero, the boss is destroyed and the level is completed. The bossObject collisions work differently in order to make this work. When the projectiles hit the boss, 
the counter gets lower and lower. The main difference being that instead of a direct destroy event, its almost the sense of there being an objective to reach before the 
destroy event can be fulfilled. The boss "arena" as I call it, is designed as such that it encourages the player to move around on the different platforms to avoid getting
hit and to continue to get more ammo for their weapons. This is one of my favorite projects so far and I feel like I'm only just getting started!
