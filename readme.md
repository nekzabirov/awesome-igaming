# Awesome iGaming [![Awesome](https://awesome.re/badge.svg)](https://awesome.re)

> A curated list of open-source software, specifications, and resources for building iGaming, online casino, and sports betting platforms.

iGaming engineering sits at the intersection of high-throughput payments, real-time game integrations, regulatory compliance, and live operational risk. Until recently most stacks were closed source. This list collects the open building blocks that exist today and the standards every operator deals with.

## Contents

- [Game Engines](#game-engines)
- [Game Aggregators](#game-aggregators)
- [Casino Lobby and Backend](#casino-lobby-and-backend)
- [Slot Machines](#slot-machines)
- [Poker](#poker)
- [Sports Betting and Sportsbook](#sports-betting-and-sportsbook)
- [Provably Fair and RNG](#provably-fair-and-rng)
- [General Game Backends](#general-game-backends)
- [Specifications and Regulatory Standards](#specifications-and-regulatory-standards)
- [Game Provider Documentation](#game-provider-documentation)
- [Related Lists](#related-lists)
- [Contributing](#contributing)

## Game Engines

The core service that owns sessions, rounds, bets, settlements, and integrations with game providers.

- [Casino Engine](https://github.com/nekzabirov/IGaming-Game-Engine) - Production-grade iGaming/casino engine in Kotlin/Ktor. Aggregator integrations (Pragmatic Play, OneGameHub, Pateplay), betting lifecycle (place/settle/rollback) with idempotency, freespin mechanics, gRPC API, RabbitMQ events. Hexagonal architecture with DDD and CQRS. Apache 2.0.

## Game Aggregators

Services that normalize many game providers behind a single API. Operators integrate the aggregator once and gain access to dozens of vendors.

- [Valkyrie](https://github.com/valkyrie-fnd/valkyrie) - Open-source game aggregator in Go. MIT License.
- [FiversCan](https://github.com/zeusbyte/FiversCan) - iGaming panel and game aggregator API in JavaScript.
- [NexusGGR Casino API](https://github.com/NexusGGR/casino-api) - Casino API integrating slots, live casino, and sports providers.

## Casino Lobby and Backend

Player-facing lobby applications and supporting backends.

- [Laravel Social Gaming](https://github.com/promexdotme/laravel-social-gaming) - Open-source social gaming engine on Laravel 11 for retro slots and RNG arcade platforms.
- [GoldenX Casino Site](https://github.com/MortalSoft/GoldenX-CASINO-SITE) - All-in-one online casino software with customizable games and SEO-optimized design.
- [Bowie Backend](https://github.com/ryan-west-casino/bowie-backend) - Backend for a casino lobby application.

## Slot Machines

Slot game implementations, math models, and simulators.

- [Cherry Charm](https://github.com/michaelkolesidis/cherry-charm) - Online 3D slot machine in Three.js and React.
- [Slot Machine Simulation](https://github.com/x4g2/slot-machine-simulation) - C++ slot machine simulation using Monte Carlo methods to estimate RTP, hit frequency, and volatility.

## Poker

Poker engines, solvers, and bot frameworks.

- [Texas Holdem Solver (Java)](https://github.com/bupticybee/TexasHoldemSolverJava) - Java-implemented Texas Holdem and Short Deck solver.
- [PyPokerEngine](https://github.com/ishikota/PyPokerEngine) - Poker engine for poker AI development in Python.
- [Texas Holdem Game Engine](https://github.com/NikolayIT/TexasHoldemGameEngine) - C# Texas Hold'em poker game engine.

## Sports Betting and Sportsbook

Sportsbook backends, odds tooling, and betting platforms.

- [Ultrabet](https://github.com/anssip/ultrabet) - Sports betting backend in Kotlin with GraphQL.
- [Ultrabet UI](https://github.com/anssip/ultrabet-ui) - Sports betting Next.js frontend, companion to Ultrabet.
- [SportsBook](https://github.com/Pringleman83/SportsBook) - Sports data scraping and analysis tool in Python.
- [Odds-API MCP Server](https://github.com/odds-api-io/odds-api-mcp-server) - MCP server that exposes real-time betting odds, events, and results from the Odds-API service to AI assistants. Covers 265+ bookmakers across 34 sports, with a free tier for development.

## Provably Fair and RNG

Random number generation and provably-fair primitives used in crypto and regulated gambling.

- [ProbablyFair](https://github.com/hexafluoride/ProbablyFair) - High-performance provably-fair RNG suited for gambling, in C#.
- [Provably Fair RNG](https://github.com/dinethlive/provably-fair-rng) - Regulator-credible, open-source RNG for online gambling, in TypeScript.

## General Game Backends

Not iGaming-specific, but useful for casino-adjacent social games, leaderboards, matchmaking, and chat.

- [Nakama](https://github.com/heroiclabs/nakama) - Scalable open-source game backend server with multiplayer, matchmaking, leaderboards, chat, and social features.

## Specifications and Regulatory Standards

The technical standards every operator and integrator works against. Most are not open licensed but are publicly readable.

- [GLI-19: Standards for Interactive Gaming Systems](https://gaminglabs.com/standards-and-certifications/) - Gaming Laboratories International standard for online casino systems.
- [GLI-33: Event Wagering Systems](https://gaminglabs.com/standards-and-certifications/) - GLI standard for sports betting and event wagering systems.
- [UKGC Remote Gambling and Software Technical Standards (RTS)](https://www.gamblingcommission.gov.uk/licensees-and-businesses/guide/remote-technical-standards) - UK Gambling Commission technical standards for remote gambling software.
- [Malta Gaming Authority Technical Standards](https://www.mga.org.mt/) - MGA regulatory and technical framework for licensed operators.
- [eCOGRA Safe and Fair Standards](https://ecogra.org/) - Independent testing and standards body for online gambling.

## Game Provider Documentation

Public docs for major game providers, useful when implementing aggregator adapters.

- [Pragmatic Play](https://www.pragmaticplay.com/) - Slots, live casino, bingo.
- [Evolution Gaming](https://www.evolution.com/) - Live casino games.
- [Playtech](https://www.playtech.com/) - Casino, poker, bingo, sports.
- [NetEnt](https://www.netent.com/) - Slot games.
- [Microgaming (Games Global)](https://www.gamesglobal.com/) - Slots, poker, and aggregation.

## Related Lists

Adjacent awesome lists that intersect with iGaming engineering.

- [awesome-software-architecture](https://github.com/mehdihadeli/awesome-software-architecture) - Hexagonal, CQRS, event-driven, and gRPC pattern catalogs where iGaming projects often appear.
- [awesome-ddd](https://github.com/heynickc/awesome-ddd) - Domain-Driven Design resources and sample projects in many languages.
- [awesome-grpc](https://github.com/grpc-ecosystem/awesome-grpc) - gRPC libraries, tools, and examples.
- [awesome-kotlin](https://github.com/Heapy/awesome-kotlin) - Kotlin frameworks, libraries, and projects.
- [awesome-ktor](https://github.com/mjovanc/awesome-ktor) - Resources for the Ktor framework ecosystem.
- [awesome-cqrs-event-sourcing](https://github.com/leandrocp/awesome-cqrs-event-sourcing) - CQRS and Event Sourcing resources.

## Contributing

Contributions are welcome. Please read the [contribution guidelines](contributing.md) before submitting a pull request.

## License

[![CC0](https://mirrors.creativecommons.org/presskit/buttons/88x31/svg/cc-zero.svg)](https://creativecommons.org/publicdomain/zero/1.0/)

To the extent possible under law, the maintainers have waived all copyright and related or neighboring rights to this work.
