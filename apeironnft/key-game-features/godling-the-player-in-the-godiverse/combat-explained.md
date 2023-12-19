---
description: How to Fight
---

# Combat Explained

<figure><img src="../../../.gitbook/assets/image (114).png" alt=""><figcaption><p>A Mage Apostle casts a spell.</p></figcaption></figure>

This page will explain how Apeiron's real-time card-battling combat system works.&#x20;

### Key Concepts

* **The Avatar** — Fully controllable, and the most important unit on the battlefield. **LOSING YOUR AVATAR MEANS YOU LOSE THE BATTLE**.
* **Apostles** — Semi-controllable units that assist Avatar. Will move and auto-attack on their own, but players can use skills to control them.&#x20;
* **Battle Team** — A team consists of one Avatar and up to four Apostles.
* **Battle Deck** — A combination of skill cards from the Avatar and Apostles. Each unit is able to bring 3 skill cards into battle, resulting in a 15 card deck (3 skill cards for Avatar, 12 for the four Apostles).

Once a battle has started, players will be whisked away to the battle map, and the battle will commence. There are 3 phases to each battle:

1. **Deployment Phase**\
   a. Position units strategically on your half of the battlefield\
   b. Draw 4 cards from shuffled deck as your starting hand
2. **Battle Phase**\
   a. Cards in hand are played by spending mana. \
   b. Play out skills, maneuver your Avatar, take down the enemy
3. **End Phase**\
   a. The end of the battle will happen when either the opposing Avatar is defeated.

**Mana** — Mana is shared among all five units, and is used to play cards from hand. Every card has a mana cost — if you don’t have enough mana to pay the cost, you can’t play the card. Additionally, when the mana bar is full, any new mana generated is lost. Make sure to spend your mana!

**Energy** — Each unit has an energy bar beneath its HP bar. It starts at 0 and goes up to 100. Dealing or taking damage generates energy, and once a unit becomes energized (by reaching max energy), it will auto-cast a special ability based on its class (if Apostle) and Planet Type (if Avatar).&#x20;

Once a unit has reached maximum energy (becomes energized), it will auto-cast a special ability. Once the ability has been used, energy will go back to 0.

**Deck**  — A deck consists of 15 cards, each card corresponding to a specific unit. Players draw 4 cards from the shuffled deck at the start of the battle. Players can always see the card on top of their deck.

After a card is played, the player will automatically draw a new card. If the deck is empty, then the discarded cards are shuffled into the deck and the player draws.

**Discard** — Players looking for a specific skill at a key moment may choose to discard a card. Discarding a card costs 1 mana, and then a new card is immediately drawn from the top of the draw pile.

**Apostle Death** — When an Apostle dies, its corresponding skill cards will be greyed out and leave the deck.&#x20;

{% embed url="https://www.youtube.com/watch?v=8aBd7eZoQms" %}
Fanmade video introducing the basics of the battle system in our PvE dungeon
{% endembed %}

### Stats

**Primary Stats**

1. Health\
   Unit starts with its maximum HP. Taking damage reduces HP. Reaching 0 HP results in death. When an Avatar dies, that player loses the game. When an Apostle dies, it leaves the battlefield and the player can no longer access its skill cards.
2. Attack (ATK)\
   Determines the power of basic auto-attacks. Many physical skills also scale with Attack. Units with higher ATK deal more physical damage in general.
3. Attack Speed\
   Represents the number of basic auto-attacks made per second.
4. Intelligence (INT)\
   Determines the power of certain skills. Many magical skills scale with Intelligence. Units with higher INT deal more magical damage in general.
5. Defence (DEF)\
   Reduces physical damage taken and is related to a concept called “damage modifier.” The damage modifier = 100 / (Defence + 100). 0 Defence means taking direct damage without any damage reduction, 100 Defence leads to a damage modifier value of 0.5, hence taking only 50% damage compared to 0 Defence.
6. Resistance (RES)\
   Similar to defence. Reduces magical damage taken, although the damage modifier is slightly different:

<figure><img src="https://miro.medium.com/v2/resize:fit:529/1*alq7gvHpVWQtVl68QQ1dJw.jpeg" alt=""><figcaption></figcaption></figure>

<figure><img src="../../../.gitbook/assets/image (24).png" alt=""><figcaption></figcaption></figure>

**Secondary Stats**

1. Attack Range\
   Determines the distance at which a unit can initiate a basic attack on an enemy. Units can attack without moving as long as the enemy is within range. Apostles outside of Attack Range will automatically seek out the closest enemy to attack.
2. Movement\
   Determines how fast units move across the battlefield.
3. Critical Chance\
   Probability of triggering a critical strike via basic attack, which deals higher damage than ATK.&#x20;
4. Critical Damage\
   Represented in % of ATK. It shows the damage of a critical strike. Default is 150%.
5. Tenacity\
   Reduces the duration of most crowd control status effects, in terms of percentage.
6. Vamp\
   Percentage of the damage done that heals the damage dealer.
