Vue 3 - Typescript 

- [Installed dependencies + configurations](#installed-dependencies--configurations)
  - [*Vue 3**](#vue-3)
  - [Possible issues](#possible-issues)

Starter projects with different dependencies and setups, ready to use

# Installed dependencies + configurations

## *Vue 3**

Command:
**npm init vue@latest**

Chosen CLI install options:

- Typescript
- Vitest
- Vue Router
- Pinia
- Eslint (code quality)
- Prettier (formatting)

(no changes to tsconfig)

## Possible issues

- Volar (plugin in vscode) may make error when using interface for props in a component, which seems due
  to the tsconfig setup which is adapted to vitest (vitest is chosen in the installation of vue as an option).
