---
title: Compression Dynamo
nav: thermal-expansion
image:
  - alt: Compression dynamo
    file: thermal-expansion/dynamo-compression-rf.png
  - alt: Compression dynamo with boiler conversion
    file: thermal-expansion/dynamo-compression-steam.png
redirect_from:
  - /docs/thermal-expansion/dynamos/compression-dynamo/
  - /docs/compression-dynamo/
recipes:
  crafting:
    - te5-dynamo-compression
augments:
  - dynamo-power
  - dynamo-efficiency
  - dynamo-coil-duct
  - dynamo-throttle
  - dynamo-boiler
  - dynamo-compression-coolant
  - dynamo-compression-fuel
  - dynamo-compression-biofuel
---

A **compression dynamo** is a [dynamo](/docs/thermal-expansion/dynamos/) fueled by fluid fuel and
[coolant](/docs/thermal-expansion/coolants/).


Obtaining
---------

A placed compression dynamo can be instantly picked up by dismantling it with a
[wrench](/docs/wrenches/). Its configuration is preserved in the item. It can
also be mined using a [pickaxe](https://minecraft.gamepedia.com/Pickaxe), though
this can be much slower.

### Crafting
{% include recipe-table.html type='crafting' recipes=page.recipes.crafting no-result=true %}

### Upgrading
A compression dynamo is initially at the lowest [tier](#tiers) (basic). It can
be upgraded to higher tiers using [upgrade kits](/docs/thermal-foundation/upgrade-kits/) and
[conversion kits](/docs/thermal-foundation/conversion-kits/).


Usage
-----

### Placement
When placed, a compression dynamo faces up. When placed while sneaking, it faces
away from the player. A compression dynamo can face any direction, and can be
rotated using a [wrench](/docs/wrenches/).

### Energy generation
When a compression dynamo is filled with fluid [fuel](#fuels) and
[coolant](/docs/thermal-expansion/coolants/), it will start consuming both to
generate [Redstone Flux](/docs/redstone-flux/). Fuel and coolant are consumed in
batches of 100 mB. Every batch of fuel yields a certain amount of energy when
consumed. Every batch of coolant can be used to generate a certain amount of
energy; this amount is equal to the [thermal
capacity](/docs/thermal-expansion/coolants/#usage) of the used coolant.

A compression dynamo generates more energy from the same amount of fuel when
stronger coolants are used. The amount of energy generated from each batch of
fuel is increased by the [coolant
factor](/docs/thermal-expansion/coolants/#usage) of the used coolant minus 20%
(the coolant factor of [water](https://minecraft.gamepedia.com/Water)). For
example, using a coolant with a coolant factor of 50% increases the amount of
energy generated by 30%. The energy increase percentage is added to the energy
increase/decrease percentages of any installed [augments](#augmentation) before
being applied to the amount of energy.

The speed at which energy is generated and fuel and coolant are consumed depends
on how much power can be emitted, and on the dynamo's maximum power output. A
basic compression dynamo has a maximum power output of 40 RF/t. This can be
increased by upgrading the dynamo to a higher [tier](#tiers), and by installing
certain [augments](#augmentation).

When an active compression dynamo cannot emit the energy it generates, it will
keep working at its minimum power output (a tenth of its maximum power output).
Any more energy that is generated in this case is lost. This can be resolved by
installing an [excitation field
limiter](/docs/thermal-expansion/augment-excitation-field-limiter/).

### Input and output
A compression dynamo emits [Redstone Flux](/docs/redstone-flux/) from its coil,
which points in the direction the dynamo is facing. It only emits energy when it
is active. Fluids can enter a compression dynamo through its sides. They cannot
enter it through the coil, unless [transmission coil
ducting](/docs/thermal-expansion/augment-transmission-coil-ducting/) is installed.

### Redstone control
A compression dynamo may be configured to respond to
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

When a compression dynamo is deactivated by a redstone signal and is still
generating energy from a consumed batch of fuel, it will finish generating
energy from that batch first.

### Security
A compression dynamo can have a [signalum security
lock](/docs/thermal-foundation/signalum-security-lock/) installed to restrict who can access it.

### Redprints
A compression dynamo's configuration can be saved on a
[redprint](/docs/thermal-foundation/redprint/) to be copied to other dynamos.

### Light source
When a compression dynamo that produces [Redstone Flux](/docs/redstone-flux/) is
active, it emits a light level of 7.


Tiers
-----

Compression dynamos come in six [tiers](/docs/thermal-foundation/tiers/).

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

A compression dynamo can have [augments](/docs/thermal-expansion/augments/) installed to improve
certain properties or to change how it works. The amount of augments that can be
installed depends on the dynamo's [tier](#tiers). A basic compression dynamo
cannot be augmented.

Augments can be installed in the Augmentation tab in a compression dynamo's GUI.

{% include augment-table.html augments=page.augments %}


Fuels
-----

The following fluids can be consumed by a compression dynamo to generate varying
amounts of energy.

| Fuel | Energy per 1,000 mB |
|---
| [Creosote Oil](/docs/thermal-foundation/creosote-oil/) | 40,000 RF |
| [Seed Oil](/docs/thermal-foundation/seed-oil/) | 80,000 RF |
| [Liquifacted Coal](/docs/thermal-foundation/liquifacted-coal/) | 400,000 RF |
| [Crude Oil](/docs/thermal-foundation/crude-oil/) | 400,000 RF |
| [Tree Oil](/docs/thermal-foundation/tree-oil/) | 400,000 RF |
| [Grassoline](/docs/thermal-foundation/grassoline/) | 800,000 RF |
| [Naphtha](/docs/thermal-foundation/naphtha/) | 1,000,000 RF |
| [Refined Fuel](/docs/thermal-foundation/refined-fuel/) | 1,500,000 RF |
| Gaseous Fuel ([BuildCraft](https://www.mod-buildcraft.com/)) | 200,000 RF |
| Mixed Light Fuels ([BuildCraft](https://www.mod-buildcraft.com/)) | 320,000 RF |
| Distilled Oil ([BuildCraft](https://www.mod-buildcraft.com/)) | 400,000 RF |
| Mixed Heavy Fuels ([BuildCraft](https://www.mod-buildcraft.com/)) | 640,000 RF |
| Light Fuel ([BuildCraft](https://www.mod-buildcraft.com/)) | 800,000 RF |
| Heavy Oil ([BuildCraft](https://www.mod-buildcraft.com/)) | 1,000,000 RF |
| Dense Oil ([BuildCraft](https://www.mod-buildcraft.com/)) | 1,600,000 RF |
| Dense Fuel ([BuildCraft](https://www.mod-buildcraft.com/)) | 2,400,000 RF |
| Canola Oil ([Actually Additions](https://minecraft.curseforge.com/projects/actually-additions)) | 80,000 RF |
| Oil ([Actually Additions](https://minecraft.curseforge.com/projects/actually-additions)) | 200,000 RF |
| Crystallized Oil ([Actually Additions](https://minecraft.curseforge.com/projects/actually-additions)) | 400,000 RF |
| Empowered Oil ([Actually Additions](https://minecraft.curseforge.com/projects/actually-additions)) | 700,000 RF |
| Hootch ([Ender IO](http://enderio.com/)) | 300,000 RF |
| Fire Water ([Ender IO](http://enderio.com/)) | 750,000 RF |
| Rocket Fuel ([Ender IO](http://enderio.com/)) | 1,000,000 RF |
| Ethanol ([Forestry](https://forestryforminecraft.info/)) | 500,000 RF |
| Biodiesel ([Immersive Engineering](https://mods.curse.com/mc-mods/minecraft/231951-immersive-engineering)) | 500,000 RF |
| Crude Oil ([Immersive Petroleum](https://minecraft.curseforge.com/projects/immersive-petroleum)) | 400,000 RF |
| Diesel ([Immersive Petroleum](https://minecraft.curseforge.com/projects/immersive-petroleum)) | 800,000 RF |
| Gasoline ([Immersive Petroleum](https://minecraft.curseforge.com/projects/immersive-petroleum)) | 1,200,000 RF |
| Biogas ([IndustrialCraft²](https://www.industrial-craft.net/)) | 50,000 RF |
{:.uk-table .uk-table-striped .uk-table-condensed .uk-text-small .cofh-table-compress}
