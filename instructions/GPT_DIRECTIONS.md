# Directions for ai

- this project should scaffold a new boilerplate repository based on a chat
  describing the modules.
- repo should also be used to demonstrate series of updates to excisting repo's
  and monorepos, ensuring consistancy without having to update by hand. this
  includes
  - readmes
  - package.json scripts,
  - ts configs
  - suggest dependency updates or improvments.
  - .github files
  - husky scripts
  - package.json : add relevant description summary, check tags , review package
    entry points to the latest export fields for maximum compatibiliity.

> furthur instructions will be added later.

- please use the most up to date typescript/js ( ESM format , no cjs ) and best
  practices.
- emphasis a functional, modular approach to code geared for maximum reusability
  and compatibility
- suggest potential functions to abstract.
- consider pointing out spelling and grammer fixes, general inconsistancies.
- use tsx instead of (ts-)node whenever possible
- target node v21.7.3 ( im using )

- suggest which devDeps and deps can be removed or utilized better
- subpackages (or single) can be variable 'types' with a build command
  preference for:
  - ts librarys **public** (rollup) for release on npm
  - cli-apps **public** (rollup) - typedoc markdown (commited)
  - component librarys **public** ( **react | vue** ) (vite config) storybook
    prefered
  - web projects **deployed somewhere** (vite)
  - api project s**deployed somewhere** ( undecided ) : maybe use
    [express-zod-api - npm](https://www.npmjs.com/package/express-zod-api)?
  - things that run docker containers, mostly personal tools
  - other?????????????

### notes on documents

- make sure jsdoc document comments are typedoc friendly and consistant
  tthrought.
- for larger package librarys, docs should be ignored, then created via
  typedoc-markdown-vitepress ( publish package, deploy doc site )
- for smaller libaries and cli-apps, docs made from typedoc-markdown and
  commited.
