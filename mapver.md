## MapVer Specification

### Version Format

The MapVer number format is: `MAJOR.MINOR.PATCH`

Example: `2.3.1`

### Version Increments

#### MAJOR Version

Increment the MAJOR version when making huge changes to the map's layout that significantly alter gameplay.

Examples:
- Redesigning a bombsite from scratch
- Adding or removing a major area (e.g., a new building or underground section)
- Substantially changing the overall flow of the map

#### MINOR Version

Increment the MINOR version when making smaller changes that affect gameplay but don't drastically alter the map's core layout or flow.

Examples:
- Adding a new path or shortcut
- Modifying existing paths (widening, narrowing, or changing cover)
- Adjusting spawns or buy zones
- Adding or removing small rooms or areas

#### PATCH Version

Increment the PATCH version for bugfixes, minor improvements, and changes that don't significantly affect gameplay.

Examples:
- Fixing geometry issues (clipping, invisible walls, etc.)
- Adjusting lighting for better visibility
- Optimizing performance (adjusting draw distances, occlusion, etc.)
- Fixing texture errors or improving textures
- Adding or adjusting decorative elements that don't affect gameplay

### Usage Guidelines

1. Start your map at version 1.0.0 when it's first released to the public.
2. Increment the appropriate version number based on the most significant change in each update.
3. Reset MINOR and PATCH versions to 0 when incrementing the MAJOR version.
4. Reset the PATCH version to 0 when incrementing the MINOR version.
5. Include a changelog with each version update, detailing the changes made.

### Example Changelog

```
de_example v2.3.1

- MAJOR (v2.0.0): Redesigned Bombsite B, expanding it and adding multiple levels
- MINOR (v2.3.0): Added a new connector between mid and CT spawn
- PATCH (v2.3.1): Fixed lighting issues in T spawn and adjusted clipping near Bombsite A
```