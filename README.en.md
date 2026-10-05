# Texas Holdem Poker Platform Source Code

[简体中文](README.zh-CN.md) | [繁體中文](README.zh-TW.md) | [English](README.en.md) | [GitHub Pages](https://alibabama401.github.io/Texas-Holdem-Poker-Platform-Source-Code/)

C++ callback and Protobuf reference for Texas Holdem platform research. Public files cover login and user-state callbacks, clubs, unions, private rooms, SNG/MTT configuration, poker messages, game records, and real mobile product screenshots.

> **Repository scope:** This is a partial source and protocol reference. It is not a complete buildable or production-ready poker platform. Missing items include the dependency graph, build scripts, database, service entry points, complete Unity scenes, and administration frontend.

## Product Views

<table>
<tr><td width="50%"><img src="docs/assets/screenshots/dating_new.JPG" alt="Lobby and room list" width="100%"><br><strong>Lobby and room list</strong></td><td width="50%"><img src="docs/assets/screenshots/julebu.jpg" alt="Club creation screen" width="100%"><br><strong>Club creation screen</strong></td></tr>
<tr><td width="50%"><img src="docs/assets/screenshots/lianmeg.jpg" alt="Union system interface" width="100%"><br><strong>Union system interface</strong></td><td width="50%"><img src="docs/assets/screenshots/mtt02.jpg" alt="MTT blind structure" width="100%"><br><strong>MTT blind structure</strong></td></tr>
<tr><td width="50%"><img src="docs/assets/screenshots/sirenju.jpg" alt="Friends-only private room" width="100%"><br><strong>Friends-only private room</strong></td><td width="50%"><img src="docs/assets/screenshots/youxi.JPG" alt="Texas Holdem game interface" width="100%"><br><strong>Texas Holdem game interface</strong></td></tr>
</table>

## Verifiable Features

- **C++ router callbacks:** login-token results, connection mapping, user metadata, online/offline state, room-status lookup, logout, and assistant-status callbacks.
- **Club and union protocols:** create, join, search, review, membership, role changes, funds, bills, tables, and union membership messages.
- **Tournament configuration:** MTT/SNG room types, blind structures, entry fees, rewards, rankings, rebuy, and refund fields.
- **Texas Holdem resources:** poker messages in `dz.proto`, records in `GameRecord.proto`, and user/club data in `Friends.proto`.
- **Product media:** 12 local screenshots plus a repository video showing lobby, club, union, tournament, private-room, and table interfaces.

## Texas Hold’em Gameplay

Each player receives two private cards. Five community cards appear across the flop, turn, and river. Betting rounds allow checking, calling, raising, or folding. The strongest five-card combination from seven available cards wins according to the table rules. The repository also contains protocol fields for SNG and MTT tournament flows.

## Source Map

| Public file | Verifiable content |
|---|---|
| `AsyncLoginCallback.*` | Login response, connection mapping, state notifications |
| `AsyncGetUserCallback.*` | Device, platform, channel, area, and robot metadata |
| `AsyncUserServerMapCallback.*` | Online/offline and room-status callbacks |
| `CommonStruct.proto` | Club, union, tournament, private-room, and coin-flow enums |
| `config.proto` | Room, MTT/SNG, blind, entry-fee, reward, and club settings |
| `dz.proto` / `GameRecord.proto` | Poker protocol fields and hand-record structures |

## Repository Layout

`*.cpp / *.h` C++ callback fragments  
`*.proto` Protobuf message definitions  
`docs/` multilingual GitHub Pages and search files  
`docs/assets/screenshots/` local product screenshots  

## Evaluation Checklist

1. Inspect `SOURCE-INVENTORY.md` and the public files.
2. Resolve missing headers, generated Protobuf/Tars code, libraries, and service implementations.
3. Document the database, deployment topology, configuration, security model, and test strategy.
4. Review `License.md`; its MIT text and separate commercial/all-rights-reserved wording should be clarified by the owner.
5. Confirm local laws, platform rules, security, and game fairness before any production use.

## Contact

Email: ttpoker40@gmail.com  
Telegram: [@alibabama401](https://t.me/alibabama401)

## Search Terms

Texas Holdem source code, C++ poker server, Protobuf poker protocol, poker club source code, private room poker, SNG, MTT, multiplayer poker.
