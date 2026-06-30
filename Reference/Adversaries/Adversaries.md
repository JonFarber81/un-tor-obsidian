---

---
This file contains adversaries from the TOR Core Rules. Stat blocks are rendered by the TOR 2E Statblocks plugin.

Shared category abilities (e.g. Hate Sunlight for all Orcs, Hideous Toughness for all Trolls) are included in each individual block to make them self-contained at the table.

# Evil Men

## Hostile Southerners

```tor2e
name: Southerner Raider
description: A marauder from the South, assembling war parties to plunder isolated homesteads.
features:
- Canny
- Hardened
level: 4
endurance: 16
might: 1
resolve: 4
parry: '+1'
armour: 2d
proficiencies:
- name: Axe
  rating: 3
  damage: 5
  injury: 18
  special: ''
- name: Short Spear
  rating: 2
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Fierce Folk. Spend 1 Resolve to gain (1d) and make the attack roll Favoured.'
```

^SouthernRaider

```tor2e
name: Southerner Champion
description: A chieftain from Dunland or bandit lord capable of uniting fractious warriors.
features:
- Cruel
- Tough
level: 5
endurance: 20
might: 1
resolve: 5
parry: '+2'
armour: 3d
proficiencies:
- name: Spear
  rating: 3
  damage: 4
  injury: 14
  special: Pierce
- name: Long-hafted Axe
  rating: 3
  damage: 6
  injury: 18
  special: Break Shield
abilities:
- 'Fierce Folk. Spend 1 Resolve to gain (1d) on an attack and to make the roll Favoured.'
```

^SouthernChampion

## Ruffians

```tor2e
name: Footpad
description: A cowardly bandit, ready to rob a defenceless victim or ambush a lonely companion.
features:
- Nimble
- Wary
level: 2
endurance: 8
might: 1
resolve: 2
parry: '—'
armour: 1d
proficiencies:
- name: Cudgel
  rating: 2
  damage: 3
  injury: 12
  special: ''
- name: Bow
  rating: 2
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Craven. When affected by the Intimidate Foe combat task, the creature also loses 1 Resolve.'
```

^Footpad

```tor2e
name: Ruffian Chief
description: A ruffian who has reached the top with a sharper mind, or blade.
features:
- Ruthless
- Secretive
level: 3
endurance: 12
might: 1
resolve: 3
parry: '+1'
armour: 2d
proficiencies:
- name: Short Sword
  rating: 3
  damage: 3
  injury: 16
  special: ''
- name: Bow
  rating: 2
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Yell of Triumph. Spend 1 Resolve to restore 1 Resolve to all other Ruffians in the fight.'
```

^RuffianChief

```tor2e
name: Highway Robber
description: A brigand used to life in the Wild, experienced at dealing with armed victims.
features:
- Swift
- Vengeful
level: 4
endurance: 16
might: 1
resolve: 4
parry: '—'
armour: 2d
proficiencies:
- name: Spear
  rating: 3
  damage: 4
  injury: 14
  special: Pierce
- name: Bow
  rating: 2
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Snake-like Speed. When targeted by an attack, spend 1 Resolve to make the attack roll Ill-favoured.'
```

^HighwayRobber

# Orcs

All Orcs suffer badly from direct sunlight and possess the **Hate Sunlight** ability (loses 1 Hate each round exposed to full sunlight). Some Orcs may also have the **Hatred (subject)** ability — when targeting the object of their hate, all attacks are Favoured.

## Great Orcs

```tor2e
name: Great Orc Chief
description: A leader and chieftain among Great Orcs, often the largest in the warband.
features:
- Bold
- Cunning
level: 7
endurance: 48
might: 2
hate: 7
parry: '+3'
armour: 4d
proficiencies:
- name: Heavy Scimitar
  rating: 3
  damage: 5
  injury: 18
  special: Break Shield
- name: Broad-headed Spear
  rating: 3
  damage: 5
  injury: 16
  special: Pierce
abilities:
- 'Horrible Strength. If the creature scored a Piercing Blow with a close combat attack, spend 1 Hate to make the target''s Protection roll Ill-favoured.'
- 'Snake-like Speed. When targeted by an attack, spend 1 Hate to make the attack roll Ill-favoured.'
- 'Yell of Triumph. Spend 1 Hate to restore 1 Hate to all other Orcs in the fight.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^GreatOrcChief

```tor2e
name: Great Orc Bodyguard
description: A fell creature that protects Orc captains at the cost of its own life.
features:
- Fierce
- Wary
level: 6
endurance: 24
might: 2
hate: 6
parry: '+2'
armour: 3d
proficiencies:
- name: Orc-axe
  rating: 3
  damage: 3
  injury: 18
  special: Break Shield
- name: Broad-headed Spear
  rating: 3
  damage: 5
  injury: 16
  special: Pierce
abilities:
- 'Hideous Toughness. When an attack inflicts damage that would cause it to go to zero Endurance, it causes a Piercing Blow instead. Then, if the creature is still alive, it returns to full Endurance.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^GreatOrcBodyguard

## Orcs of the North

```tor2e
name: Goblin Archer
description: An Orc chosen for keen eyes, shooting with precision by night or day.
features:
- Cunning
- Keen-eyed
level: 2
endurance: 8
might: 1
hate: 2
parry: '—'
armour: 1d
proficiencies:
- name: Bow of Horn
  rating: 3
  damage: 3
  injury: 14
  special: Pierce
- name: Jagged Knife
  rating: 2
  damage: 2
  injury: 14
  special: ''
abilities:
- 'Craven. When affected by the Intimidate Foe combat task, the creature also loses 1 Hate.'
- 'Orc-poison. If an attack results in a Wound, the target is also poisoned.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^GoblinArcher

```tor2e
name: Orc-chieftain
description: The most wicked and cruel Orcs, wielding the meanest weapons and superior armour.
features:
- Cruel
- Hardened
level: 5
endurance: 20
might: 1
hate: 5
parry: '+3'
armour: 3d
proficiencies:
- name: Scimitar
  rating: 3
  damage: 3
  injury: 16
  special: ''
- name: Spear
  rating: 3
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Great Leap. Spend 1 Hate to attack any Player-hero, in any combat stance, including Rearward.'
- 'Snake-like Speed. When targeted by an attack, spend 1 Hate to make the attack roll Ill-favoured.'
- 'Yell of Triumph. Spend 1 Hate to restore 1 Hate to all other Orcs in the fight.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^OrcChieftain

```tor2e
name: Orc Guard
description: The strongest and boldest Orcs, equipped with the toughest armour set to watch key areas.
features:
- Strong
- Vigilant
level: 4
endurance: 16
might: 1
hate: 4
parry: '+2'
armour: 3d
proficiencies:
- name: Scimitar
  rating: 3
  damage: 3
  injury: 16
  special: ''
- name: Spear
  rating: 3
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^OrcGuard

```tor2e
name: Orc Soldier
description: A loud and undisciplined Orc, kept in line only by a forceful chieftain.
features:
- Rebellious
- Vengeful
level: 3
endurance: 12
might: 1
hate: 3
parry: '+1'
armour: 2d
proficiencies:
- name: Scimitar
  rating: 3
  damage: 3
  injury: 16
  special: ''
- name: Spear
  rating: 2
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Craven. At the start of the round, the adversary flees the battlefield if at zero Hate and is unengaged.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^OrcSoldier

# Trolls

All Trolls possess **Hideous Toughness** (when damage would reduce them to zero Endurance, it causes a Piercing Blow instead; if still alive, returns to full Endurance) and **Dull-witted** (Player-heroes in Forward stance may make a RIDDLE roll as their main action; on a success the Troll loses 1 Hate plus 1 per Success icon rolled). All Trolls also suffer from **Hate Sunlight**.

## Cave-trolls

Cave-trolls cannot endure sunlight and never leave their underground hunting grounds.

```tor2e
name: Great Cave-troll
description: A massive Troll sent by Orcs to smash defences and shatter the morale of foes.
features:
- Brutish
- Wicked
level: 10
endurance: 80
might: 2
hate: 10
parry: '—'
armour: 3d
proficiencies:
- name: Crush
  rating: 3
  damage: 6
  injury: 12
  special: Seize
- name: Bite
  rating: 2
  damage: 6
  injury: 14
  special: Pierce
abilities:
- 'Strike Fear. Spend 1 Hate to make all Player-heroes in sight gain 3 Shadow points (Dread). Those who fail their Shadow test are daunted and cannot spend Hope for the rest of the fight.'
- 'Thick Hide. Spend 1 Hate to gain (2d) on a Protection roll.'
- 'Hideous Toughness. When an attack inflicts damage that would cause it to go to zero Endurance, it causes a Piercing Blow instead. Then, if still alive, it returns to full Endurance.'
- 'Dull-witted. A Player-hero in Forward stance may make a RIDDLE roll as their main action; on a success the Troll loses 1 Hate, plus 1 per Success icon rolled.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^GreatCaveTroll

```tor2e
name: Cave-troll Slinker
description: A smaller Cave-troll that hunts alone in darkness, guided by an acute sense of smell.
features:
- Stealthy
- Wary
level: 6
endurance: 50
might: 2
hate: 6
parry: '—'
armour: 3d
proficiencies:
- name: Club
  rating: 3
  damage: 6
  injury: 16
  special: Break Shield
- name: Bite
  rating: 2
  damage: 6
  injury: 14
  special: Pierce
abilities:
- 'Denizen of the Dark. All attack rolls are Favoured while in darkness.'
- 'Fear of Fire. The creature loses 1 Hate at the start of each round it is engaged in close combat with an adversary wielding a torch or other burning item.'
- 'Thick Hide. Spend 1 Hate to gain (2d) on a Protection roll.'
- 'Hideous Toughness. When an attack inflicts damage that would cause it to go to zero Endurance, it causes a Piercing Blow instead. Then, if still alive, it returns to full Endurance.'
- 'Dull-witted. A Player-hero in Forward stance may make a RIDDLE roll as their main action; on a success the Troll loses 1 Hate, plus 1 per Success icon rolled.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun.'
```

^CaveTrollSlinker

## Stone-trolls

Stone-trolls turn to stone if exposed to direct sunlight. They particularly hate Dwarves.

```tor2e
name: Stone-troll Robber
description: A Stone-troll that wears clothes and uses tools, prowling near populated areas.
features:
- Hungry
- Irritable
level: 8
endurance: 60
might: 2
hate: 8
parry: '—'
armour: 3d
proficiencies:
- name: Club
  rating: 3
  damage: 6
  injury: 16
  special: Break Shield
- name: Crush
  rating: 2
  damage: 6
  injury: 12
  special: Seize
abilities:
- 'Hatred (Dwarves). When fighting Dwarves, all the creature''s rolls are Favoured.'
- 'Horrible Strength. If the creature scores a Piercing Blow, spend 1 Hate to make the target''s Protection roll Ill-favoured.'
- 'Hideous Toughness. When an attack inflicts damage that would cause it to go to zero Endurance, it causes a Piercing Blow instead. Then, if still alive, it returns to full Endurance.'
- 'Dull-witted. A Player-hero in Forward stance may make a RIDDLE roll as their main action; on a success the Troll loses 1 Hate, plus 1 per Success icon rolled.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun (and turns to stone in direct sunlight).'
```

^StoneTrollRobber

```tor2e
name: Stone-troll Chief
description: A stronger Stone-troll around which small groups band together to attack caravans.
features:
- Cruel
- Suspicious
level: 9
endurance: 70
might: 2
hate: 9
parry: '—'
armour: 3d
proficiencies:
- name: Club
  rating: 3
  damage: 6
  injury: 16
  special: Break Shield
- name: Crush
  rating: 2
  damage: 6
  injury: 12
  special: Seize
abilities:
- 'Hatred (Dwarves). When fighting Dwarves, all the creature''s rolls are Favoured.'
- 'Horrible Strength. If the creature scores a Piercing Blow, spend 1 Hate to make the target''s Protection roll Ill-favoured.'
- 'Yell of Triumph. Spend 1 Hate to restore 1 Hate to all other Trolls in the fight.'
- 'Hideous Toughness. When an attack inflicts damage that would cause it to go to zero Endurance, it causes a Piercing Blow instead. Then, if still alive, it returns to full Endurance.'
- 'Dull-witted. A Player-hero in Forward stance may make a RIDDLE roll as their main action; on a success the Troll loses 1 Hate, plus 1 per Success icon rolled.'
- 'Hate Sunlight. The creature loses 1 Hate for each round it is exposed to the full light of the sun (and turns to stone in direct sunlight).'
```

^StoneTrollChief

# Undead

All Undead possess three shared abilities: **Deathless** (spend 1 Hate to cancel a Wound; when damage would reduce to zero Endurance, spend 1 Hate to return to full Endurance instead — ineffective against weapons enchanted for the Bane of the Undead), **Heartless** (not affected by Intimidate Foe unless a Magical success is obtained), and **Strike Fear** (spend 1 Hate to make all Player-heroes in sight gain 3 Shadow points Dread; those who fail their Shadow test are daunted and cannot spend Hope for the rest of the fight).

## Wights

```tor2e
name: Barrow-wight
description: A tall, dark figure with cold eyes lit by pale light, sent to haunt the barrow-downs.
features:
- Cunning
- Vengeful
level: 6
endurance: 24
might: 1
hate: 6
parry: '—'
armour: 3d
proficiencies:
- name: Ancient Sword
  rating: 3
  damage: 5
  injury: 16
  special: Pierce
- name: Chilling Touch
  rating: 2
  damage: 6
  injury: 12
  special: Seize
abilities:
- 'Denizen of the Dark. All attack rolls are Favoured while in darkness.'
- 'Dreadful Spells. Spend 1 Hate to make one Player-hero gain 3 Shadow points (Sorcery). Those who fail their Shadow test or are Miserable fall unconscious; may only be roused with a SONG roll, otherwise wake after one hour.'
- 'Hate Sunlight. The creature loses 1 Hate at the start of each round it is exposed to the full light of the sun.'
- 'Deathless. Spend 1 Hate to cancel a Wound. When damage would cause it to go to zero Endurance, spend 1 Hate to return to full Endurance instead. Ineffective against weapons enchanted for the Bane of the Undead.'
- 'Heartless. Not affected by the Intimidate Foe combat task unless a Magical success is obtained.'
- 'Strike Fear. Spend 1 Hate to make all Player-heroes in sight gain 3 Shadow points (Dread). Those who fail their Shadow test are daunted and cannot spend Hope for the rest of the fight.'
```

^BarrowWight

## Wraiths

```tor2e
name: Fell Wraith
description: A crooked wanderer in ancient cloaks, a creature whose life was consumed by sorcery.
features:
- Swift
- Wary
level: 4
endurance: 16
might: 1
hate: 4
parry: '+1'
armour: 2d
proficiencies:
- name: Pitted Blade
  rating: 3
  damage: 4
  injury: 16
  special: ''
- name: Cruel Spear
  rating: 2
  damage: 4
  injury: 14
  special: Pierce
abilities:
- 'Denizen of the Dark. All attack rolls are Favoured while in darkness.'
- 'Fear of Fire. The creature loses 1 Hate at the start of each round it is engaged in close combat with an adversary wielding a torch or other burning item.'
- 'Deathless. Spend 1 Hate to cancel a Wound. When damage would cause it to go to zero Endurance, spend 1 Hate to return to full Endurance instead. Ineffective against weapons enchanted for the Bane of the Undead.'
- 'Heartless. Not affected by the Intimidate Foe combat task unless a Magical success is obtained.'
- 'Strike Fear. Spend 1 Hate to make all Player-heroes in sight gain 3 Shadow points (Dread). Those who fail their Shadow test are daunted and cannot spend Hope for the rest of the fight.'
```

^FellWraith

```tor2e
name: Marsh Dwellers
description: Shambling humanoid creatures with clammy flesh, lurking in ruins near stagnant pools.
features:
- Fierce
- Stealthy
level: 3
endurance: 12
might: 1
hate: 3
parry: '—'
armour: 1d
proficiencies:
- name: Bite
  rating: 3
  damage: 3
  injury: 14
  special: Pierce
- name: Claws
  rating: 2
  damage: 3
  injury: 14
  special: Seize
abilities:
- 'Fear of Fire. The creature loses 1 Hate at the start of each round it is engaged in close combat with an adversary wielding a torch or other burning item.'
- 'Hate Sunlight. The creature loses 1 Hate at the start of each round it is exposed to the full light of the sun.'
- 'Deathless. Spend 1 Hate to cancel a Wound. When damage would cause it to go to zero Endurance, spend 1 Hate to return to full Endurance instead. Ineffective against weapons enchanted for the Bane of the Undead.'
- 'Heartless. Not affected by the Intimidate Foe combat task unless a Magical success is obtained.'
- 'Strike Fear. Spend 1 Hate to make all Player-heroes in sight gain 3 Shadow points (Dread). Those who fail their Shadow test are daunted and cannot spend Hope for the rest of the fight.'
```

^MarshDwellers

# Wolves of the Wild

All Wolves of the Wild share **Great Leap** (spend 1 Hate to attack any Player-hero, in any combat stance, including Rearward).

## Wargs

```tor2e
name: Wild Wolf
description: A particularly evil Warg, slightly larger than an ordinary wolf and much more vicious.
features:
- Keen-eyed
- Grim
level: 3
endurance: 12
might: 1
hate: 3
parry: '—'
armour: 1d
proficiencies:
- name: Fangs
  rating: 3
  damage: 3
  injury: 14
  special: Pierce
abilities:
- 'Fear of Fire. The creature loses 1 Hate at the start of each round it is engaged in close combat with an adversary wielding a torch or other burning item.'
- 'Snake-like Speed. When targeted by an attack, spend 1 Hate to make the attack roll Ill-favoured.'
- 'Great Leap. Spend 1 Hate to attack any Player-hero, in any combat stance, including Rearward.'
```

^WildWolf

```tor2e
name: Wolf-chieftain
description: Greater in stature and cunning than ordinary Wargs, never encountered alone.
features:
- Swift
- Vicious
level: 4
endurance: 16
might: 1
hate: 4
parry: '—'
armour: 1d
proficiencies:
- name: Fangs
  rating: 3
  damage: 4
  injury: 14
  special: Pierce
- name: Claws
  rating: 2
  damage: 4
  injury: 14
  special: Seize
abilities:
- 'Fear of Fire. The creature loses 1 Hate at the start of each round it is engaged in close combat with an adversary wielding a torch or other burning item.'
- 'Snake-like Speed. When targeted by an attack, spend 1 Hate to make the attack roll Ill-favoured.'
- 'Howl of Triumph. Spend 1 Hate to restore 1 Hate to all other Wargs in the fight.'
- 'Great Leap. Spend 1 Hate to attack any Player-hero, in any combat stance, including Rearward.'
```

^WolfChieftain

## Werewolves

```tor2e
name: Hound of Sauron
description: A trusted servant of the Dark Lord in wolf-form, sent on precise errands of the Dark Lord.
features:
- Cunning
- Fierce
level: 5
endurance: 20
might: 2
hate: 5
parry: '+1'
armour: 2d
proficiencies:
- name: Fangs
  rating: 3
  damage: 5
  injury: 14
  special: Pierce
- name: Claws
  rating: 3
  damage: 5
  injury: 14
  special: Seize
abilities:
- 'Deadly Wound. Wounded targets make an Ill-favoured Feat die roll to determine the severity of their injury.'
- 'Hideous Toughness. When an attack inflicts damage that would cause it to go to zero Endurance, it causes a Piercing Blow instead. Then, if still alive, it returns to full Endurance.'
- 'Strike Fear. Spend 1 Hate to make all Player-heroes in sight gain 3 Shadow points (Dread). Those who fail their Shadow test are daunted and cannot spend Hope for the rest of the fight.'
- 'Great Leap. Spend 1 Hate to attack any Player-hero, in any combat stance, including Rearward.'
```

^HoundOfSauron
