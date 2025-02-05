---
title: Steam Dynamo
nav: thermal-expansion
image:
  - alt: Steam dynamo
    file: thermal-expansion/dynamo-steam-rf.png
  - alt: Steam dynamo with boiler conversion
    file: thermal-expansion/dynamo-steam-steam.png
redirect_from:
  - /docs/thermal-expansion/dynamos/steam-dynamo/
  - /docs/steam-dynamo/
recipes:
  crafting:
    - te5-dynamo-steam
augments:
  - dynamo-power
  - dynamo-efficiency
  - dynamo-coil-duct
  - dynamo-throttle
  - dynamo-boiler
  - dynamo-steam-turbine
---

A **steam dynamo** is a [dynamo](/docs/thermal-expansion/dynamos/) fueled by
[water](https://minecraft.gamepedia.com/Water) and solid fuel.


Obtaining
---------

A placed steam dynamo can be instantly picked up by dismantling it with a
[wrench](/docs/wrenches/). Its configuration is preserved in the item. It can
also be mined using a [pickaxe](https://minecraft.gamepedia.com/Pickaxe), though
this can be much slower.

### Crafting
{% include recipe-table.html type='crafting' recipes=page.recipes.crafting no-result=true %}

### Upgrading
A steam dynamo is initially at the lowest [tier](#tiers) (basic). It can be
upgraded to higher tiers using [upgrade kits](/docs/thermal-foundation/upgrade-kits/) and
[conversion kits](/docs/thermal-foundation/conversion-kits/).


Usage
-----

### Placement
When placed, a steam dynamo faces up. When placed while sneaking, it faces away
from the player. A steam dynamo can face any direction, and can be rotated using
a [wrench](/docs/wrenches/).

### Energy generation
A steam dynamo has a fuel slot and a
[water](https://minecraft.gamepedia.com/Water) tank. When [fuel](#fuels) is
placed in its fuel slot and the tank is filled with water, the dynamo will start
consuming both to generate [Redstone Flux](/docs/redstone-flux/). Every unit of
fuel yields a certain amount of energy when consumed. Water is consumed in
batches of 100 mB to generate 25,000 RF at a time.

The speed at which energy is generated and fuel is consumed depends on how much
power can be emitted, and on the dynamo's maximum power output. A basic steam
dynamo has a maximum power output of 40 RF/t. This can be increased by upgrading
the dynamo to a higher [tier](#tiers), and by installing certain
[augments](#augmentation).

When an active steam dynamo cannot emit the energy it generates, it will keep
working at its minimum power output (a tenth of its maximum power output). Any
more energy that is generated in this case is lost. This can be resolved by
installing an [excitation field
limiter](/docs/thermal-expansion/augment-excitation-field-limiter/).

### Input and output
A steam dynamo emits [Redstone Flux](/docs/redstone-flux/) from its coil, which
points in the direction the dynamo is facing. It only emits energy when it is
active. Fuel and water can enter a steam dynamo through its sides. They cannot
enter it through the coil, unless [transmission coil
ducting](/docs/thermal-expansion/augment-transmission-coil-ducting/) is installed.

### Redstone control
A steam dynamo may be configured to respond to
[redstone](https://minecraft.gamepedia.com/Redstone) signals. It can be in one
of three modes:

Ignored
: Redstone control is disabled. The dynamo works whenever possible. This is the
default mode.

Low
: The dynamo works when *not* powered. When powered, it stops working.

High
: The dynamo only works when powered.

The current mode can be set using the Redstone Control tab in the dynamo's GUI.

When a steam dynamo is deactivated by a redstone signal and is still generating
energy from a consumed unit of fuel, it will finish generating energy from that
unit of fuel first.

### Security
A steam dynamo can have a [signalum security
lock](/docs/thermal-foundation/signalum-security-lock/) installed to restrict who can access it.

### Redprints
A steam dynamo's configuration can be saved on a [redprint](/docs/thermal-foundation/redprint/) to
be copied to other dynamos.

### Light source
When a steam dynamo that produces [Redstone Flux](/docs/redstone-flux/) is
active, it emits a light level of 7.


Tiers
-----

Steam dynamos come in six [tiers](/docs/thermal-foundation/tiers/).

{::options parse_block_html="true" /}
<div class="uk-overflow-container">
| Tier | Max. power output | Augment slots |
|---
| Basic | 40 RF/t | 0 |
| Hardened | 60 RF/t | 1 |
| Reinforced | 80 RF/t | 2 |
| Signalum | 100 RF/t | 3 |
| Resonant / Creative | 120 RF/t | 4 |
{:.uk-table .uk-table-striped .uk-table-condensed .uk-text-small .cofh-table-compress}
</div>
{::options parse_block_html="false" /}


Augmentation
------------

A steam dynamo can have [augments](/docs/thermal-expansion/augments/) installed to improve certain
properties or to change how it works. The amount of augments that can be
installed depends on the dynamo's [tier](#tiers). A basic steam dynamo cannot be
augmented.

Augments can be installed in the Augmentation tab in a steam dynamo's GUI.

{% include augment-table.html augments=page.augments %}


Fuels
-----

A steam dynamo accepts all items that can be used as fuel in a
[furnace](https://minecraft.gamepedia.com/Furnace), except for those that leave
items in a furnace's fuel slot after being consumed, like [lava
buckets](https://minecraft.gamepedia.com/Lava_Bucket).

| Fuel | Energy per unit |
|---
| [Coal](https://minecraft.gamepedia.com/Coal) | 24,000 RF |
| [Block of Coal](https://minecraft.gamepedia.com/Block_of_Coal) | 240,000 RF |
| [Pulverized Coal](/docs/thermal-foundation/pulverized-coal/) | 24,000 RF |
| [Charcoal](https://minecraft.gamepedia.com/Charcoal) | 16,000 RF |
| [Block of Charcoal](/docs/thermal-foundation/block-of-charcoal/) | 160,000 RF |
| [Pulverized Charcoal](/docs/thermal-foundation/pulverized-charcoal/) | 16,000 RF |
| [Coal Coke](/docs/thermal-foundation/coal-coke/) | 40,000 RF |
| [Block of Coal Coke](/docs/thermal-foundation/block-of-coal-coke/) | 400,000 RF |
| Any other [furnace](https://minecraft.gamepedia.com/Furnace) fuel* | (Burn time in ticks × 10) RF
{:.uk-table .uk-table-striped .uk-table-condensed .uk-text-small .cofh-table-compress}

*: Items with very short burn times (less than 300 ticks) cannot be used as
fuel.
