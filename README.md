# Defold TypeScript Template (minimal - Bun version)

<a href="https://discord.gg/eukcq5m"><img alt="Chat with us!" src="https://img.shields.io/discord/766898804896038942.svg?colorB=7581dc&logo=discord&logoColor=white"></a> [![CI/CD](https://github.com/thinknathan/tsd-template-bun/actions/workflows/build.yml/badge.svg)](https://github.com/thinknathan/tsd-template-bun/actions/workflows/build.yml) ![GitHub License](https://img.shields.io/github/license/thinknathan/tsd-template-bun)

A dev environment for [Defold](https://defold.com/) that transpiles TypeScript into lua using [TypeScriptToLua](https://github.com/TypeScriptToLua/TypeScriptToLua) 
and [Bun](https://bun.sh/).

## Features

- Full Lua and Defold API type definitions for TypeScript auto-complete and type checking
- Library of types for Defold extensions via `bun run resolve`
- Eslint config for handling the caveats of TypeScriptToLua and keeping your code correct
- Handles script, gui_script, and module exports using familiar ES6 export syntax
- Full BoilerPlate game project ready to transpile and go
- File watcher via `bun run dev` to transpile on save

_Note that you will need to have [Bun](https://bun.sh/) installed._

## Quick Start

- Use `bun run dev` to start a watcher that compiles and emits lua and script when you save
- Use `bun run build` to just compile your ts, sans watcher

## Installation

1. Fork this template or use [degit](https://www.npmjs.com/package/degit) to download the template locally

```bash
npx degit thinknathan/tsd-template-bun my-game
# or
git clone https://github.com/thinknathan/tsd-template-bun.git my-game
```

2. Initialize

```bash
cd my-game
bun install
```

3. Generate

```bash
bun run build # Transpile the TypeScript files to lua
# or
bun run dev # Watch for changes and regenerate files on save
```

4. Code

```
code .
```

5. Open `app/game.project` in Defold

- Start making games with TypesScript!

<p align="center" class="h4">
  TypeScript :heart: Defold
</p>
