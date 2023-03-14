# Dungeon Master
A project detailing the game Dungeon Master which is an original idea for a game by Johnathan of Nichathan Gaming.

## Table of Contents
1. **[Introduction](#Introduction)**
2. **[Backstory](#Backstory)**
3. **[Unsorted Ideas](#Unsorted-Ideas)**
4. **[Game Outline](#Game-Outline)**
    1. **[Objective](#Objective)**
    2. **[Currencies](#Currencies)**
    3. **[Room types](#Room-types)**
    4. **[Dungeon Functions and events](#Dungeon-Functions-and-events)**
        1. **[Delivery](#Delivery)**
        2. **[Special Guest](#Special-Guest)**
        3. **[Appearances](#Appearances)**
    5. **[Monster Skills](#Monster-Skills)**
    6. **[Hero spells](#Hero-spells)**
5. **[List of Room Names](#List-of-Room-Names)**
6. **[Game Design - GUI](#Game-Design-GUI)**

## Introduction
Dungeon master is a fun and unique android game designed by Johnathan from Nichathan Gaming where the player builds a dungeon to save monsters.
</br>**[Back to top](#Dungeon-Master)**

## Backstory
You were once the master of the largest and most successful dungeon in the world. Monsters were thriving and humanity was on the brink of extinction. As an imortal being at the height of your power with nothing left to do, you took a nap. 
1000 years later, you awake to find that your once glorious dungeon has collapsed in on itself. Even worse, humanity has made a comeback and they are now terrorizing monsters everywhere. 
Will you be able to restore your dungeon back to its former glory or will your reign end with a thud?
You decide.
</br>**[Back to top](#Dungeon-Master)**

## Unsorted Ideas
1. When you want to remove a monster from your dungeon, the room that they are in must not be producing goods at the time. Also, the button will say "Send to fight the hero". After clicking this button, there is a verification screen that says "Are you sure, [MonsterName] will not return from this mission."
2. Whenever a special guest is created, reduces the current chance to have another show up - down to a 5% chance. Whenever a normal guest is created, increases the current chance that a special guest will show up - up to the maximum chance.
3. Let's have a living quarters room that actually has "living quarters". 
</br>![image](https://user-images.githubusercontent.com/103794085/224879439-fe2b775f-4522-45a0-8705-b44b7966211d.png)
</br>**[Back to top](#Dungeon-Master)**

## Game Outline
### Objective
The objective of the game is to build a thriving dungeon. With each new floor that you build, you must choose one of 6 different room types. All of which have their own unique bonuses. As you play, you will earn Copper Coins and Dungeon Dollars which can be used to further upgrade your dungeon.
</br>**[Back to top](#Dungeon-Master)**

### Currencies
This game has 2 currencies: 
1. Copper Coins - As the base currency of the game, Copper Coins are used to : 
    1. Purchase new dungeon levels
    2. Unlocking certain dungeon master spells 
    3. Much more...
2. Dungeon Dollars - The elite currency of the game which can only be obtained by spending real money or by chance through completing special missions. You can use Dungeon Dollars for many things including but not limited to : 
    1. Purchasing Copper Coins
    2. Buying special monsters
    3. Unlocking certain dungeon master spells
    4. Buying special rooms
    5. Rearranging rooms
    6. Upgrading characters 
    7. Much more...
</br>**[Back to top](#Dungeon-Master)**

### Room types
There are 6 room types which each have their own benefits:
1. Living quarters : Holds up to 6 monsters and allows them to work in your dungeon. Be careful however because when a hero arrives in the dungeon, he can kill these monsters.
2. Food : These rooms provide food for the monsters in your dungeon. They produce goods the fastest but provide the least amount of Copper Coins per good sold. You receive a small boost to production speed.
		  </br>- Speed 5, Value 1
3. Recreation : These rooms allow your monsters to relax and focus more on work when they go back. They provide a small boost to the health of your monsters and reduce the speed that a hero can steal your gold at.
		  </br>- Speed 4, Value 2
4. Mystic : These rooms control the mystic forces within the dungeon. The more of them that you have, the more dungeon master skills will be unlocked. Skills are unlocked randomly and may cost Copper Coins or Dungeon Dollars to activate/upgrade. These rooms also increase the chance of special deliveries.
		  </br>- Speed 3, Value 3
5. Armory : These rooms prepare your monsters for combat. For each room of this type in your dungeon, you may earn more dungeon dollars and coins from every interaction.
		  </br>- Speed 2, Value 4
6. Beastiary :  These rooms house large monsters in your dungeon. Large monsters are the way that monsters can move around in your dungeon. For each Beasteary in your dungeon, you can upgrade the speed of your elevator (This is done by unlocking the option to permanantly hire a faster large monster to work as your elevator.)
		  </br>- Speed 1, Value 5
</br>**[Back to top](#Dungeon-Master)**

### Dungeon Functions and events
#### Delivery
The player will frequently `(randomly once every 30 seconds to 2 minutes)` be asked to transport a monster to a random floor of your dungeon. This monster is just a visitor and they will pay the dungeon master `(1 Copper Coin * (number of levels travelled-1))*(number of Armories +1)`.
If the passenger arrives at a Living Quarters room with an empty space, then they will join the dungeon and not pay any money.
</br>**[Back to top](#Dungeon-Master)**

#### Special Guest
There is a `(10% + (1% * number of mystics))` chance to have a special guest instead of the normal monster for delivery. When a special guest appears in the elevator, the game will produce a pop-up that tells the player what their speciality is. The player can then choose to use the guest, send up to 5 of them to the waiting room, or if no room is left in the waiting room, send to attack the city.
</br>Special Guests : 
1. Pied Piper - fills up a living quarters room with random monsters - `17% chance`
2. Tycoon - purchases all of the merchandice in a level. - `17% chance`
3. Factory Executive - fills up the stock of a single level. - `16% chance`
4. Tourist - (highest chance of spawning) can be taken to any room and gives double the normal delivery fee - `26% chance`
5. Mover - allows whichever room he is delivered to to be moved one time. - `14% chance`
6. Designer - Provides a free room upgrade to whichever room he is taken to - `10% chance`
</br>**[Back to top](#Dungeon-Master)**

#### Appearances 
While playing the game, once every `3-5` minutes, a special event will happen where a one of the following happens :
1. **Hero attack** - A hero enters your dungeon and begins attacking your monster. Each monster has `100hp` and the hero deals `10 damage every 5-10 seconds`. Monsters heal `1%` of their HP every minute. The hero will continue attacking until all employed monsters on a floor have been killed or until the player clicks on them. The player can spend 1 Dungeon Dollar to revive a dead monster to 50% hp. Clicking on the hero gives `((1-2) * number of armories)` dungeon dollars.
2. Hero steal - A hero enters your dungeon and begins stealing your Copper Coins. The hero steals `0.1%` of your gold every `5-10` seconds at a minimum of 1 Copper Coin per cycle. The hero will stay until 10% of your Copper Coins is gone or he has been clicked. The Copper Coins stolen are non-returnable but the player gains `((1-2) *number of Armories)` Dungeon Dollars when clicking on the hero.
3. Lost Monster - A monster is somewhere in your dungeon. He will give `50%` chance that you will receive a special guest until a special guest is spawned. This chance drops by `1% every 5-10` seconds that the monster is not found. If the chance reaches 0, the monster goes away. You also gain `((1-2) * number of armories)` Dungeon Dollars when clickinig on the lost monster.
</br>**[Back to top](#Dungeon-Master)**

### Monster Skills
Each monster that permantly joins the dungeon by moving into the living quarters will have a preferred room to work in.
On top of this, monsters will have random skills for each room type. These skills range from 1-9. The higher the number, the faster they produce items in a room. If they are sent to their preferred room, they will produce 2 times faster and sell items for 2 times more.
Monsters come in 5 types :
1. Exceptional - These monsters have 2 skills of level `8-9` and random numbers for their other skills of `1-9` - `5% chance`
2. Great - These monsters have 1 skill that is from level `7-9` and another from `6-9` with the last 3 being random from `1-9` - `15% chance`
3. Average - These monsters have an equal chance that all skills be 1 or 9. Skills range from `1-9` - `50% chance`
4. Below Average - These monsters have 1 skill that is from `1-3` and another from `5-8` with the last 3 being random from `1-9`- `20% chance`
5. Poor - These monsters have 2 skills of level `1-2` and random numbers for their other skills of `1-5` - `10% chance`
</br>**[Back to top](#Dungeon-Master)**

### Hero spells
1. Increase Copper Coin generation - Copper Coins
2. Increase Dungeon Dollars generation - Dungeon Dollars
3. Increase production speen in room type 1-5 - Copper Coins
4. Increase sale value in room type 1-5 - Dungeon Dollars
5. Reduces the cost increase after purchasing a new floor - Dungeon Dollars
6. Increase the elevator speed - Copper Coins
7. Increase Appearance chance - Dungeon Dollars
8. Increase Special Guest chance - Copper Coins
9. Reduce the hero effectiveness - Copper Coins
10. Increase the chance of a new monster having higher skills - Dungeon Dollars
</br>**[Back to top](#Dungeon-Master)**

## List of Room Names
Each of the 6 room types has 10 different rooms that the monsters pick a favorite from randomly. The player can purchase a specific room for 100 Dungeon Dollars. Or 25, if the room has already been made. When creating new rooms, rooms that have been created already will not naturally be recreated, they must be purchased to have duplicates of a room.
1. Living quarters
      1. Undecided
      2. Undecided
      3. Undecided
      4. Undecided
      5. Undecided
      6. Undecided
      7. Undecided
      8. Undecided
      9. Undecided
      10. Undecided
2. Food 
      1. Undecided
      2. Undecided
      3. Undecided
      4. Undecided
      5. Undecided
      6. Undecided
      7. Undecided
      8. Undecided
      9. Undecided
      10. Undecided
3. Recreation
      1. Undecided
      2. Undecided
      3. Undecided
      4. Undecided
      5. Undecided
      6. Undecided
      7. Undecided
      8. Undecided
      9. Undecided
      10. Undecided
4. Mystic
      1. Undecided
      2. Undecided
      3. Undecided
      4. Undecided
      5. Undecided
      6. Undecided
      7. Undecided
      8. Undecided
      9. Undecided
      10. Undecided
5. Armory
      1. Undecided
      2. Undecided
      3. Undecided
      4. Undecided
      5. Undecided
      6. Undecided
      7. Undecided
      8. Undecided
      9. Undecided
      10. Undecided
6. Beastiary
      1. Undecided
      2. Undecided
      3. Undecided
      4. Undecided
      5. Undecided
      6. Undecided
      7. Undecided
      8. Undecided
      9. Undecided
      10. Undecided
</br>**[Back to top](#Dungeon-Master)**

## Game Design-GUI
The game design for the GUI has not been made yet however, as I imagine it, it will look like this:
1. A pixelated 2D platformer city is at the top of the screen. Heroes can be seen wandering here and there will be occasional fights with monsters that have no bearing on the actual game, it just makes things more interesting.
2. On the right of the screen (outside of the city), you see a cave opening. Directly below that cave, there is a tunnel with a large lizard like monster with a cage on its back. - This is the elevator and the skin and speed changes as the player upgrades it.
3. Directly under the city, the player sees a cavernous waiting area. This is the area where up to 5 special guests can be saved for later. - Heroes never show up here.
4. At the very bottom of the dungeon, you can see a large monster digging out the next room. This animation is repeated indefinitely until the player purchases the next room with Copper Coins.
5. Each room of the same name will have a unique design to it. Each room type will have an animation for the 3 employed monsters to perform indefinitely.
6. If a room does not have an employee, it will be greyed out and there will be an exclamation mark in the top left corner of that room. If a room is out of supplies, it will be greyed out. If a room is producing supplies, there will be an icon for that supply as well as a loading bar that shows the player how much longer it will take before the item is produced as well as an hour / minute timer. If production has finished in a room, there will be an icon that the player must press to pick up the produced items so they can be sold. If a room has an employee that loves the job, there will be a star for each employee that loves the room and is working there by the elevator. If all 3 employees love the room, then production and sales will be automatic and the employees can be moved at any time.
</br>**Very Rough Sketch**
</br>![image](https://user-images.githubusercontent.com/103794085/224889551-67d9ab18-e3a8-4819-bf36-3d6d3120be25.png)

</br>**[Back to top](#Dungeon-Master)**
