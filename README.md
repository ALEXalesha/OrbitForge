<div align="center">

# OrbitForge

**Build rockets from parts and fly them through a real-scale Solar System in 3D. Full n-body gravity, atmosphere and reentry heating, time warp, crews on EVA, rovers, planes, stations and a career - on Unity 6 HDRP.**

[Русская версия этого файла](README.ru.md)

[![Status](https://img.shields.io/badge/status-in_development-orange)](#) [![License](https://img.shields.io/badge/license-MIT-blue)](LICENSE) [![Unity](https://img.shields.io/badge/Unity_6-HDRP-000000?logo=unity&logoColor=white)](https://unity.com/) [![C#](https://img.shields.io/badge/C%23-239120?logo=csharp&logoColor=white)](https://learn.microsoft.com/dotnet/csharp/) [![Blender](https://img.shields.io/badge/Blender-models-F5792A?logo=blender&logoColor=white)](https://www.blender.org/) [![Built with Claude Code](https://img.shields.io/badge/Built_with-Claude_Code-D97757?logo=claude&logoColor=white)](https://claude.com/claude-code)

Code, tests and docs are written by Claude (Anthropic) in Claude Code. Ideas, testing and decisions - Alexey.

</div>

> **Status: in development, nothing to download yet.** Work started on 15 November 2026. This page describes the plan; it will get screenshots and builds as stages are finished.

## The idea

A 3D rocket-building and spaceflight game in the spirit of the genre, made from scratch with its own parts, look and interface. You design a rocket in a 3D hangar, launch it from a spaceport, reach orbit, plan maneuvers on an orbit map, fly to the Moon and the planets, land, walk outside and come back home.

## Planned

- **Hangar** - engines, tanks, fairings, legs, parachutes, docking ports, cockpits, solar panels; parametric parts (any tank size by slider); mass, thrust, TWR and Δv per stage; paint and emblems.
- **Physics** - full n-body gravity, real-size planets, double precision with a floating origin, aerodynamics, reentry heating, structural flex without "wobbly" rockets, real engines and fuels (Isp changes with altitude, hydrogen boil-off); time warp for long transfers.
- **The real Solar System** - Sun, eight planets, the Moon and major moons on real orbits; Earth with oceans, continents, clouds, night lights and atmosphere glow; planet surfaces from open height maps; day and night, eclipses, a real starry sky.
- **Flight** - orbit map with maneuver nodes, launch windows, gravity assists and Lagrange points, staging with pyro bolts and fairing shells, honest engine plumes, docking with an assistant, autopilot and flight scripts, several vessels at once, a camera feed from the rocket.
- **Crew** - EVA with a jetpack, walks on the Moon and Mars, life support and power, g-forces and crew health.
- **Rovers, planes and stations** - wheeled rovers, wing aerodynamics and spaceplanes, orbital stations and surface bases, building in space.
- **Career and sandbox** - missions, money, science instruments, research, historical missions without brands, reusable boosters, satellites and communication networks, asteroids and comets, launch-day weather, solar flares and dust storms, records and achievements, launch archive with charts, a rocket museum.
- **Cheat mode** - infinite fuel, no drag, no breaking and simplified controls, with the same good graphics.
- **Tutorial** - orbits explained step by step; in-game help in Russian and English; save anywhere and rewind.

## Tech

Unity 6 with HDRP, C#. The flight core (orbital mechanics, integrator, Δv, aerodynamics, heat, economy, saves) is plain C# without the engine and is covered by invariant tests, branch coverage and mutation testing. Models are made in Blender with code; textures are CC0 photo textures (Poly Haven, ambientCG).

## License

[MIT](LICENSE)
