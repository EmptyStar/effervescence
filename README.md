# Effervescence

Add a subtle touch of life to your world with Effervescence! This mod adds ambient particle effects to any world: bustling grasses, blossoming flowers, crumbling stone, and much more.

## Effects

Effervescence comes with the following default effects:

- **dusty** - dust particles that swirl about from dry, dusty nodes
- **crumbly** - bits of loose dirt that fall from ceilings made of stone, dirt, or moss
- **bustling** - grass, pollen, and spores that lift up from the ground
- **snowy** - snowflake squalls that gust up from the ground
- **leafy** - gently falling leaves from trees and bushes
- **blossoming** - flower petals blown away from flowers
- **sporogenic** - bursts of spores shed by mushrooms and certain types of vines and plants
- **sparkly** - fine sparkles generated by crystals and ice
- **bubbling** - tiny bubbles that form at the surface of water
- **walking** - bits of dirt and grass kicked up under players' feet as they walk

## Advanced Usage

Effervescence is actually a modpack that comes with three mods:

- The core `effervescence` mod which provides an API and trigger mechanism for particle effects
- `effervescence_decorators` which defines a set of default *decorators* used to place node metadata during mapgen
- `effervescence_particles` which defines the default particle effects bundled with Effervescence

The secondary mods can be disabled in order to remove the bundled particle effects, and the mods can be individually depended upon for adding custom particle effects or decorators. The mod settings can be used to adjust mod behavior for performance, and the API can be used to control the mod programmatically.

## Notes

- This mod is primarily targeted at [Asuna](https://content.luanti.org/packages/EmptyStar/asuna/) but will mostly work for other typical sandbox games
- This mod utilizes mapgen to determine where particles can occur in the environment which means that environmental particles will only appear in previously unexplored areas
- Particle effects will not be applied to nodes placed by players although this can be achieved by adding `effervescence.particles` node metadata, an advanced task ~~covered in the API documentation~~

## Caveats

- Particle effects may cause lag on older hardware, especially in areas with lots of dense particle-emitting nodes
- This mod adds metadata to the world to determine where particle effects can occur; uninstalling this mod will leave its metadata behind which causes no noticeable effect but will cause your world to permanently take up more space on your device
- The color of particles may be wrong for nodes that use hardware coloring