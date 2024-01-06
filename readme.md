# Mock TNT
This Minetest mod creates propulsive, blinding, but non-damaging TNT that still adds to gameplay as an alternative to TNT.


## Differences from regular TNT
* Does not destroy nodes (blocks)
* Does not cause fire
* Causes "Blind" and "Slow" conditions temporarily (if playereffects is installed)
* Does not ignite nearby TNT (*may in a later version*)

### Similarities to regular TNT
* Causes knockback: pushes player away from explosion by 1 (*may be increased in a later version*)
* Reduces HP of entities in range.


## Installation
* Place in .minetest/mods/ (or the mods/ subfolder in your game).
* Set `enable_tnt = false` in your minetest.conf
* This mod requires the tnt mod, and the playereffects mod is recommended.


## Usage
Settings: The only settings used are `enable_tnt` and `tnt_radius` that are
documented in the tnt mod (required), but the `enable_tnt` setting
impacts the mock_tnt as described below (for more documentation see
settingtypes.txt in minetest_game which is the origin of the tnt mod).

Modes:
* `enable_tnt = false` (recommended): This mod will define gunpowder and mock_tnt even if enable_tnt is false.
  - Generally, unless you set it to false, there is no point in using the mock_tnt mod except as described below for worlds that used it before.
* `enable_tnt = true` (fallback mode): mock_tnt still is defined but has no recipe. This behavior is useful if you are re-enabling regular TNT for a world that contains mock_tnt already.
  - The caption will say "Unknown Explosive" (mock_tnt:mock_tnt) and the texture will be a parody texture of "unknown item" texture (with a fuse added) so it can coexist separately from TNT when TNT is enabled.


## Known Issues
See <https://github.com/Poikilos/mock_tnt/issues>.
