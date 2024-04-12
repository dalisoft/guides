# Git PR/Branch comparison

| Feature                | Merge                   | Rebase                   | Squash                          |
| ---------------------- | ----------------------- | ------------------------ | ------------------------------- |
| Used by                | [Go-to](#merge-used-by) | [Go-to](#rebase-used-by) | [Go-to](#squash--merge-used-by) |
| Signed by GitHub       | ❌                      | ❌                       | ✅                              |
| PR testing in prod     | ❌                      | ✅                       | ⚠️                              |
| Linear history         | ❌                      | ✅                       | ⚠️                              |
| Full-commits history   | ✅                      | ✅                       | ❌                              |
| Debug / Bisect         | ✅                      | ⚠️                       | ❌                              |
| Merge commit annoyance | ✅                      | ❌                       | ❌                              |
| Auto-merge PR          | ✅                      | ❌                       | ✅                              |
| Easy Revert PR         | ✅                      | ❌                       | ✅                              |
|                        |                         |                          |                                 |
| Total score            | 5                       | 3.5                      | 4                               |

## Merge Used by

- [VSCode](https://github.com/microsoft/vscode)
- [Express.js](https://github.com/expressjs/express) **Needs confirmation**
- [Git](https://github.com/git/git)
- [Linux](https://github.com/torvalds/linux)

## Rebase Used by

- [Tensorflow](https://github.com/tensorflow/tensorflow) **Needs confirmation**

## Squash & Merge Used by

- [ESLint](https://github.com/eslint/eslint)
- [Fastify](https://github.com/fastify/fastify)
- [jQuery](https://github.com/jquery/jquery)
- [React](https://github.com/facebook/react)
- [Vue.js](https://github.com/vuejs/core)
- [Puppeteer](https://github.com/puppeteer/puppeteer)
- [Node.js](https://github.com/nodejs/node)
- [Prettier](https://github.com/prettier/prettier)
- [Biomejs](https://github.com/biomejs/biome)
- [TypeScript](https://github.com/microsoft/TypeScript)
- [ESBuild](https://github.com/evanw/esbuild)
- [Bun](https://github.com/oven-sh/bun)
