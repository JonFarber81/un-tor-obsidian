There seem to be some bugs with the dice roller plugin. Trying to sort out what works.

Lists plot threads inspired by Mythic GME.

### Rolling from Lists

- The Spider
- The Trollmen
- Dwarven Waystations

^list-test

Entry from a list: `dice: [[DiceRoller^list-test]]` after the roll. For The display shows the full list item with the bullet which I don't necessarily want. This looks particularly bad in edit mode, but not great in reader either.

When trying to return multiple results it is also a mess since the bullet formatting is not preserved.
`dice: 3d[[DiceRoller^list-test]]`
Another bug with list rollers is that after reloading obsidian, the first two entries in a list are ignored and never returned. You have to edit or move the cursor through the list for this to refresh. This seems

### Rolling from Tables

| Header | Value |
| ------ | ----- |
| A      | 1     |
| B      | 2     |
| C      | 3     |

^tableroll

Table rolling seems to match what I expect more closely: `dice: [[DiceRoller#^tableroll]]` or just one column: `dice: [[DiceRoller#^tableroll]]|Value`

- `dice: 3d[[DiceRoller#^tableroll]]|Header`

