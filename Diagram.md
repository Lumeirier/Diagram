```mermaid
graph TD;
    spawn[**SPAWN**
You awaken in a tavern room. Outside your door you hear the sounds of joyous conversation and the clinking of metal mugs.

**What do you do?**] 

    dead[**You are dead**]

    wake[**WAKE UP**
You decide to get out of bed and start your journey. You rush out the door, grabbing your sword on the way out and leave the tavern. You can go west towards the forest, or north towards the city.

**What do you do**?]

    east[**EAST**
You decide to venture east into the forest. Many monsters are said to be there. You come across a raging river.There is a log resting over it which you could cross. You could also try going around the river.

**What do you do**?]

    cross[**CROSS THE RIVER**
You take the chance to cross the log. You are midway through when you slip on some moss. You are washed away, but at least the water was refreshing.]

    around[**GO AROUND**
You decide to play it safe and go around. Unfortunately you forgot about the crypt that lay between you and the other side. An armored lich raises from the ground, greatsword in hand.

**What do you do?**]

    fight[**FIGHT**
You swing your sword at the lich, managing to take off one of its arms. The lich tries to swing its hefty greatsword at you, but stumbles. You take the chance to go for victory. Upon slaying the undead lich, you discover a chest of gold. So much gold that you are set for life.]

    retire[**RETIREMENT**
You retire with the mass amount of gold you found. You decide to start a book store, selling choose your own adventure books.]
    
    run[**RUN**
    You try to run, but trip. The lich slams the greatsword down on you and you perish, but at least you didn't feel any pain.]

    north[**NORTH**
You head north towards the city. Upon arrival, the guard asks you for your papers. You rummage through your bag, but do not find them. The guard is getting agitated and asks for your papers once more.

**What do you do**?]

    bribe[**BRIBE**
You hand the guard 5 gold coins in an attempt to get her to look the other way. You are arrested immediately. You are scheduled for execution tomorrow, but at least they're giving you a great final meal.]

    truth[**TELL THE TRUTH**
You admit to the guard that you lost your papers. She tells you that you must obtain a proper ID to enter the city, and points you to the nearest government building. You arrive at the Department of Medieval Visuals.]

    dmv[**DMV**
You wither away waiting for your ID, as there's 30 people in front of you, all waiting for their portrait to be painted. You pass away, but at least you weren't arrested.]

    sleep[
**SLEEP**
You decide this isn't worth the hassle and fall back asleep. Outside, a drunken bard falls trying to imitate a bear and catches his lute on the fireplace. The lute is lit aflame and the fire spreads from instrument to the tavern floor. As all the patrons rush to the exit and the tavernkeep weeps for his loss, you sleep peacefully through the commotion, and being cooked alive. You had a wonderful dream at least.
]


    spawn --> sleep;
    spawn --> wake;
    wake --> east;
    wake --> north;
    east --> cross;
    cross --> dead;
    east --> around;
    around --> fight;
    around --> run;
    fight --> retire;
    run --> dead;
    north --> bribe;
    north --> truth;
    bribe --> dead;
    truth --> dmv;
    dmv --> dead;
    cross --> dead
    sleep --> dead;
    dead --> spawn;
```

### Documentation

> This is a choose-your-own adventure story! I used a flow chart to create a dialogue tree to create the branching paths the reader could choose. Each entity is pretty self explanatory and is a piece of narrative used as part of the whole tree. Each piece on it's own doesn't make much sense, but the whole comes together to form a little story the reader can interact with.

>Each dialogue option gives significance by directly impacting the next branches. For example, choosing to wake up versus staying asleep marks either the continuation of the story or its abrupt end. Each entity supports the entire narrative by each being a core part of the dialogue tree.
