# Contributing to deployments-manual

The whole manual lives in [README.md](README.md). There is no code, build or test setup.

## How the README is organized

- A short intro: every example assumes the app is built into `dist/`.
- A table of contents linking to each platform.
- One `##` section per platform, with an emoji at the end of the heading, numbered steps (install the CLI, log in, build, deploy) and a `Docs:` link to the platform's official getting-started page.

## Adding a platform

1. Add a `## <Platform> <emoji>` section next to the other platforms.
2. Write the steps as a numbered list with the exact commands in backticks. Keep `dist/` as the output directory.
3. If the platform has more than one way to deploy (for example drag & drop and CLI), split them into "Option 1" and "Option 2".
4. End the section with a `Docs:` link to the official documentation.
5. Add the platform to the table of contents. GitHub builds the anchor from the heading, including a trailing `-` for the emoji (for example `#netlify-`).

## Conventions

- Format Markdown with Prettier: `npx prettier --write README.md CONTRIBUTING.md`.
- Commit messages follow Conventional Commits (`docs: ...`).
