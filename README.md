echo "# AstroDB Issue: Cannot find module 'astro:db'

This repository is a minimal reproduction of an issue where files outside the \`./src\` directory cannot find the \`astro:db\` module or its corresponding type declarations.

## Steps to reproduce

1. Clone this repository
2. Run \`yarn install\` (or \`npm install\`)
3. Observe that files in the \`./src\` directory can import from \`astro:db\` without issues
4. Try to import from \`astro:db\` in a file outside \`./src\`, such as \`db/config.ts\`
5. Observe the error: \`cannot find module 'astro:db' or its corresponding type declarations\`

## Expected behavior

Files outside the \`./src\` directory should be able to import from \`astro:db\` without issues.

## Actual behavior

Files outside the \`./src\` directory produce an error when trying to import from \`astro:db\`.

## Environment

- Astro version: 5.0.0-beta.4
- Node version: v20.3.1
- Package manager: yarn 4.5.0
