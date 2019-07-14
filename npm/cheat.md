# Npm Cheatsheet

Npm stuff I don't want to forget.

## Commands

- `npm outdated`
  - Show table of outdated dependencies.

## Link

- Directions:
  1. Run `npm link` inside of the package you want to link to.
  2. Run `npm link my-package` inside the project you want to link from.
- Pitfalls:
  - Singleton dependencies shouldn't be installed in the linked-to package.
    - Example:
      - For React packages, the linked-to package shouldn't have `node_modules/react` or `node_modules/react-dom`.
  - In general, dependencies in `peerDependencies` shouldn't be installed in the linked-to package.
