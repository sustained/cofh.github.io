---
title: Blazing Pyrotheum
nav: thermal-foundation
redirect_from:
  - /thermal-expansion/fluids/blazing-pyrotheum/
  - /docs/thermal-foundation/fluids/blazing-pyrotheum/
  - /docs/thermal-foundation/fluids/elemental/blazing-pyrotheum/
  - /docs/blazing-pyrotheum/
recipes:
  crucible:
    - pyrotheum
  transposer-empty:
    - bucket-pyrotheum
usage-recipes:
  transposer-fill:
    - bucket-pyrotheum
---

![Blazing pyrotheum](/assets/images/thermal-foundation/blazing-pyrotheum.gif){:style="height: 128px"}

> This is actually worse than lava. You monster.


**Blazing pyrotheum** is the fire elemental fluid. It is obtained by melting
[pyrotheum dust](/docs/thermal-foundation/pyrotheum-dust/) in a [magma
crucible](/docs/thermal-expansion/magma-crucible/).


Obtaining
---------

### Magma Crucible
{% include recipe-table.html type='crucible-te5' recipes=page.recipes.crucible %}

### Fluid Transposer
{% include recipe-table.html type='transposer-te5-empty' recipes=page.recipes.transposer-empty %}


Usage
-----

Blazing pyrotheum can be placed as a block using a
[bucket](https://minecraft.gamepedia.com/Bucket).

### Light source
Blazing pyrotheum blocks emit a light level of 15.

### Flow
The way blazing pyrotheum flows is similar to
[lava](https://minecraft.gamepedia.com/Lava). Pyrotheum source blocks will also
gradually fall downwards if there are no blocks below them.

### Effects
Most [entities](https://minecraft.gamepedia.com/Entity) that touch blazing
pyrotheum take 2 damage every half-second.

Like [lava](https://minecraft.gamepedia.com/Lava), blazing pyrotheum starts
fires. However, pyrotheum does so much more aggressively, instantly starting
fires on top of every adjacent block.

Blazing pyrotheum has the following effects on certain blocks and mobs:

* flammable blocks are instantly destroyed;
* [cobblestone](https://minecraft.gamepedia.com/Cobblestone) is smelted into
  [stone](https://minecraft.gamepedia.com/Stone);
* [grass blocks](https://minecraft.gamepedia.com/Grass_Block) are turned into
  [dirt](https://minecraft.gamepedia.com/Dirt);
* [sand](https://minecraft.gamepedia.com/Sand) is smelted into
  [glass](https://minecraft.gamepedia.com/Glass);
* [water](https://minecraft.gamepedia.com/Water) and
  [ice](https://minecraft.gamepedia.com/Ice) is turned into
  [stone](https://minecraft.gamepedia.com/Stone);
* [clay](https://minecraft.gamepedia.com/Clay_(block)) is smelted into
  [terracotta](https://minecraft.gamepedia.com/Terracotta);
* [snow](https://minecraft.gamepedia.com/Snow_Block) and [snow
  layers](https://minecraft.gamepedia.com/Slow_(layer)) are evaporated;
* [cobblestone stairs](https://minecraft.gamepedia.com/Stairs) are smelted into
  [stone brick stairs](https://minecraft.gamepedia.com/Stairs);
* [creepers](https://minecraft.gamepedia.com/Creeper) instantly explode.


### Fluid Transposer ingredient
{% include recipe-table.html type='transposer-te5-fill' recipes=page.usage-recipes.transposer-fill %}

### Pyro-Concentrator
An [induction smelter](/docs/thermal-expansion/induction-smelter/) with a
[pyro-concentrator](/docs/thermal-expansion/augment-pyro-concentrator/) installed consumes blazing
pyrotheum to process ores more efficiently. It consumes 100 mB of pyrotheum per
processed ore.

### Magmatic Dynamo fuel
When used as fuel in a [magmatic dynamo](/docs/thermal-expansion/magmatic-dynamo/), a bucket of
blazing pyrotheum yields 2,000,000 RF, or 2,500,000 RF if an [isentropic
reservoir](/docs/thermal-expansion/augment-isentropic-reservoir/) is installed.

### Reactant Dynamo fuel
When used together with [cryotheum dust](/docs/thermal-foundation/cryotheum-dust/) as fuel in a
[reactant dynamo](/docs/thermal-expansion/reactant-dynamo/), 100 mB of blazing pyrotheum yields
400,000 RF, or 500,000 RF if an [elemental
catalyzer](/docs/thermal-expansion/augment-elemental-catalyzer/) is installed.
