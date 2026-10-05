# Public Source Inventory

This inventory describes files visible in the repository on 2026-10-05. It prevents screenshots and protocol definitions from being mistaken for a complete buildable platform.

## Present

- C++ callback fragments for login, logout, user information, online state, server mapping, and assistant status.
- Protobuf definitions for shared structures, room/tournament configuration, Texas Holdem messages, friends, and game records.
- Selected card-logic headers and implementation fragments.
- Unity folder metadata without the corresponding complete Unity project.
- Twelve Pages screenshots, ten additional table-interaction screenshots, and one product video.
- README, support, security, citation, responsible-use, and Pages files.

## Not Present or Not Verifiable

- A complete dependency graph or build definition.
- Generated Protobuf/Tars sources and all referenced headers/libraries.
- Database schema, migrations, seed data, and production configuration.
- Complete server implementations and executable entry points.
- Complete Unity scenes, scripts, assets, and build settings.
- A web client, administration frontend, payment-provider integration, or anti-cheat implementation.
- Automated tests, reproducible build evidence, deployment manifests, or release binaries.

## License Review

`License.md` contains MIT License text followed by separate commercial-license and “All Rights Reserved” wording. The repository owner should clarify the intended license before reuse or distribution.
