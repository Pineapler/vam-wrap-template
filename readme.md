# Wrap template for Virt-A-Mate characters

This is a template for wrapping the DAZ Genesis 2 Female model to a character.

## Wrapping

There are just over 200 points to place on your character's mesh. Most of them are symmetric, so it is closer to 100 manually placed points. See the [point definitions](docs/point-definitions.md) for a walkthrough of how points are defined on the G2 Female model.

## Texture transfer

Currently, texturing takes `n * m` texture transfer operations, where `n` is the number of G2 textures (usually 3) and `m` is the number of source model textures.
This will hopefully be reduced in the near future.

- Make subsets of the G2 model, one for each texture. See [materials by texture](docs/materials-by-texture.md) for a list of each material group that uses a texture.
- Make subsets of the source model, one for each texture (this is easier if materials are maintained when model is exported)
- Make `n * m` "Transfer Texture" nodes

### TODO:
- Use UDIM version of G2 Female model to reduce the number of texture transfer operations
