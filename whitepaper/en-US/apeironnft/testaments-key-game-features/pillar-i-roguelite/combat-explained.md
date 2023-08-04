# Combat Explained

<figure><img src="../../../.gitbook/assets/image (77).png" alt=""><figcaption><p>The Mage casts a spell.</p></figcaption></figure>

This page will explain how Apeiron's card-battling real-time combat system works.&#x20;

&#x20;We'll start with key concepts:

* **The Avatar** — Fully controllable, and the most important unit on the battlefield — loss of the Avatar means losing the battle.
* **Apostles** — Semi-controllable units that assist Avatar. Will move and auto-attack on their own, but will respond to players using skills.
* **Battle Team** — A full team consists of one Avatar and up to four Apostles.
* **Battle Deck** — A combination of skill cards from the Avatar and Apostles. Each unit is able to bring 3 skill cards into battle, resulting in a 15 card deck (3 skill cards for Avatar, 12 for the four Apostles).

Once a battle has started, players will be whisked away to the battle map, and the battle will commence. There are 3 phases to each battle:

1. **Deployment Phase**\
   a. Draw 4 cards from shuffled deck\
   b. Position units strategically on your half of the battlefield\
   c. In PvP, you can see the enemy team composition, but not position
2. **Battle Phase**\
   a. Lasts for a maximum of 6 minutes\
   b. Cards in hand are played by spending mana\
   c. Issue move and attack commands for your Avatar while timing skills
3. **End Phase**\
   a. The end of the battle will happen when either the opposing Avatar is dead OR the timer counts down to zero.\
   b. If the timer counts down to zero, the team with the higher health Avatar wins!

Now let’s explore some of the battle mechanics in more detail, starting with…

**Mana** — Mana is shared among all five units, and is used to play cards from hand. Each team begins with 5 mana and has a maximum capacity of 10. Mana is regenerated at a rate of 0.5 mana per second, doubling to 1 mana per second at 3 minutes (halfway into the battle).

Every card has a mana cost — if you don’t have enough mana to pay the cost, you can’t play the card. Additionally, when the mana bar is full, any new mana generated is lost. Make sure to spend your mana!

**Energy** — Each unit has an energy bar beneath its HP bar. It starts at 0 and goes up to 100. Every auto attack generates 10 energy, while every instance of damage taken generates energy equal to 20% of damage, capped at 50 energy per instance.

Once a unit has reached maximum energy (becomes energized), it will auto-cast a special ability. Once the ability has been used, energy will go back to 0.

**Deck and Skill Cards** — A deck consists of 15 cards, each card corresponding to a specific unit. Players draw 4 cards from the shuffled deck at the start of the battle. They will also be able to see the next card on top of the draw pile.

After a card is played, it is immediately replaced in the hand by the next card on top of the draw pile. If the draw pile is empty, then the discard pile is shuffled into the draw pile.

Players looking for a specific skill at a key moment may choose to discard a card. Discarding a card costs 1 mana, and then a new card is immediately drawn from the top of the draw pile.

**Apostle Death and Respawn** — When an Apostle dies, its corresponding skill cards will be greyed out and disabled until the Apostle is respawned. These cards may still be discarded. The Apostle may be respawned by spending a certain amount of mana.

Finally, let’s take a look at some of the statistics that units will have. Units will have Primary and Secondary stats. Most skill cards scale with primary stats, but some perks and passives could improve secondary stats.

**Primary Stats**

1. Health\
   Unit starts with its maximum HP. Taking damage reduces HP. Reaching 0 HP results in death. When an Avatar dies, that player loses the game. When an Apostle dies, it is withdrawn from the battlefield and can be respawned later.
2. Attack\
   Determines the power of basic attack. Many physical skills also scale with attack. Units with higher ATK deal more physical damage in general.
3. Attack Speed\
   Represents the number of basic attacks made per second.
4. Intelligence\
   Determines the power of certain skills. Many magical skills scale with intelligence. Units with higher intelligence deals more magical damage in general.
5. Defence\
   Reduces physical damage taken and is related to a concept called “damage modifier.” Damage modifier = 100 / (Defence + 100). 0 Defence means taking direct damage without any damage reduction, 100 Defence leads to a damage modifier value of 0.5, hence taking only 50% damage compared to 0 Defence.
6. Resistance\
   Similar to defence. Reduce magical damage taken.

<figure><img src="https://miro.medium.com/v2/resize:fit:529/1*alq7gvHpVWQtVl68QQ1dJw.jpeg" alt=""><figcaption></figcaption></figure>

**Secondary Stats**

1. Attack Range\
   Determines the distance at which a unit can initiate a basic attack on an enemy. Units can attack without moving as long as the enemy is within range.
2. Movement\
   Determines how fast units move across the battlefield.
3. Critical Chance\
   Probability of triggering a critical strike via basic attack, which deals higher damage than ATK. Default is 0.
4. Critical Damage\
   Represented in % of ATK. It shows the damage of a critical strike. Default is 150%.
5. Tenacity\
   Reduces the duration of most crowd control status, in terms of percentage.
6. Health Regeneration\
   The rate at which a unit’s health is naturally restored.
7. Energy Regeneration\
   The rate at which a unit’s energy is naturally restored. Default is 0.
8. Vamp\
   Percentage of the damage done that heals the damage dealer.
