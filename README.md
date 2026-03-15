# beb
> Bun, Elysia and Biome!

Highly abstracted API development template.

## Features
* [Bun](https://bun.sh/) for native Typescript support and speed.
* [Elysia](https://elysiajs.com/) is designed for humans and feels mnemonic.
* [Biome](https://biomejs.dev/) provides both formatting and linting in one unified package.

## Usage
Sensible defaults are prioritized.
```sh
# Develope
bun dev
# Release
bun build-bundle
# Start (post-release)
bun start
# Compile (bundles the Bun runtime DLL along with the code in an executable)
bun build-binary
# Typecheck
bun typecheck
# Format 
bun format
# Lint
bun lint
```
The format command will format almost everything in the project, but Biome is set to it will ignore
anything that's in `.gitignore` and any file larger then 2MB which is double the default!

It will also organize your imports, if you don't like this, you can easily change this by modifying
`biome.json`.

Linting is using the recommended settings, but is strict on unused variables and imports!

## Installation
Install [Bun](https://bun.sh/) then just:
```
git clone https://github.com/abchll/beb
cd beb
bun install && bun dev
```

> [!NOTE]
> You could modify `biome.json` by adding `"formatter.useEditorConfig": true` to
use an `.editorconfig` for formatting rules if you are into that.

## Shoutouts
I heard [Zod](https://zod.dev/) is cool!
