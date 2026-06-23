# OXY Poker

## Persistent Multi-Agent Poker Simulation Engine

OXY Poker is a simulation-first software project built around a deterministic
Texas Hold'em engine and a persistent world of autonomous player profiles.

The source repository remains private. This repository documents the verified
architecture, development process and working product.

## What the system does

- runs persistent six-player poker sessions
- maintains hero and bot profiles between sessions
- models player strategy, momentum and social relationships
- tracks leagues, standings and long-term progression
- exposes runtime state through a Flask REST API
- provides operator and player interfaces built with React
- records telemetry for hands, players and session behaviour
- supports optional AI-generated commentary and narrative layers

## Architecture

```mermaid
flowchart LR
    UI[React Interface] --> API[Flask REST API]
    API --> GAME[Poker Runtime]
    GAME --> ENGINE[Deterministic Holdem Engine]
    GAME --> PROFILES[Persistent Player Profiles]
    GAME --> SOCIAL[Social Memory]
    GAME --> LEAGUES[Leagues and Standings]
    GAME --> TELEMETRY[Runtime Telemetry]
    PROFILES --> STORAGE[(Persistent Storage)]
    SOCIAL --> STORAGE
    LEAGUES --> STORAGE
```

## Engineering priorities

- chip conservation and correct pot settlement
- legal betting actions and all-in edge cases
- deterministic engine behaviour
- stable API contracts
- separation of transient hands from persistent world state
- operator visibility through telemetry and diagnostics
- incremental development through documented checkpoints

## Development approach

OXY Poker was created through AI-assisted software development.

My responsibilities include product direction, requirements, architecture
decisions, agent coordination, acceptance testing, runtime verification and
approval of stable Git checkpoints. AI coding agents accelerate implementation,
but every delivered system is reviewed against explicit requirements.

## Technology

Python, Flask, React, Vite, REST APIs, persistent storage, automated testing,
Git and Linux.

## Current status

The engine, API, interfaces, persistent profiles, leagues, social memory and
telemetry are implemented as a working prototype.

The project remains under active development. Some older runtime components are
still being progressively modularized.

## Source availability

The production source code, runtime data, credentials and infrastructure
configuration are private. Screenshots, demonstrations and additional
architecture notes will be published here.
