# claude-md-templates

Production-ready `CLAUDE.md` templates for different project types. Copy a template, customize it, and give your AI coding assistant the context it needs to write better code.

## What is CLAUDE.md?

`CLAUDE.md` is a file that lives in your project root. [Claude Code](https://docs.anthropic.com/en/docs/claude-code) reads it automatically to understand your project's stack, architecture, conventions, and commands. Think of it as onboarding docs — but for AI.

**Without CLAUDE.md:** the AI guesses your conventions, uses wrong patterns, imports non-existent modules.

**With CLAUDE.md:** the AI follows your architecture, uses your utilities, matches your style from the first prompt.

## Templates

| Template | Stack | Best for |
|----------|-------|----------|
| [react-nextjs](templates/react-nextjs/) | Next.js 14, App Router, Tailwind, Prisma | SaaS apps, full-stack Next.js |
| [nestjs-backend](templates/nestjs-backend/) | NestJS, Clean Architecture, TypeORM/Prisma | REST APIs, microservices, DDD |
| [fullstack-monorepo](templates/fullstack-monorepo/) | Turborepo, Next.js + NestJS, shared packages | Monorepos with multiple apps |
| [react-native](templates/react-native/) | React Native, Expo, Expo Router | Cross-platform mobile apps |
| [library-npm](templates/library-npm/) | TypeScript, tsup, Vitest | npm packages, CLI tools |
| [minimal](templates/minimal/) | Any stack | Quick start, prototypes |

## Quick Start

```bash
# 1. Pick a template
cp templates/react-nextjs/CLAUDE.md your-project/CLAUDE.md

# 2. Edit the placeholders
#    Replace [Project name] and [brief description]
#    Adjust sections to match your setup

# 3. Start Claude Code in your project
cd your-project
claude
```

That's it. Claude Code picks up the file automatically.

## For Monorepos

Copy the multi-file setup:

```bash
cp templates/fullstack-monorepo/CLAUDE.md your-project/CLAUDE.md
cp templates/fullstack-monorepo/apps/web/CLAUDE.md your-project/apps/web/CLAUDE.md
cp templates/fullstack-monorepo/apps/api/CLAUDE.md your-project/apps/api/CLAUDE.md
```

Claude Code reads the nearest CLAUDE.md when you navigate between apps.

## Docs

- [Writing Guide](docs/writing-guide.md) — how to write an effective CLAUDE.md
- [Anti-Patterns](docs/anti-patterns.md) — common mistakes to avoid
- [Advanced Patterns](docs/advanced-patterns.md) — multi-file setups, dynamic context, team overrides

## Contributing

Want to add a template for Django, Go, Swift, or another stack? See [CONTRIBUTING.md](CONTRIBUTING.md).

## Author

**Alex Rogov** — Full-Stack JS Architect, Amsterdam

- Twitter: [@Alex_Rogov_js](https://x.com/Alex_Rogov_js)
- LinkedIn: [rogov-alex](https://www.linkedin.com/in/rogov-alex/)
- GitHub: [autosergach](https://github.com/autosergach)

## License

[MIT](LICENSE)
