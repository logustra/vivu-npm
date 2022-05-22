## Vivu NPM
[![License](https://img.shields.io/github/license/logustra/vivu-npm)](https://github.com/logustra/vivu-npm/blob/master/license.md)
[![Code Style](https://img.shields.io/badge/code_style-standard-brightgreen.svg)](https://standardjs.com)
[![Commitizen](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli)

> Starter template to build component library for vue.js 2-3

## Features
- Faster by default: [vite](https://github.com/vitejs/vite), [vue](https://github.com/vuejs/vue-next), [pnpm](https://github.com/pnpm/pnpm), [esbuild](https://github.com/evanw/esbuild)
- Typescript, of course
- Testing: [vitest](https://vitest.dev/)
- Git custom hooks: [husky](https://github.com/typicode/husky)
- Commit conventions: [commitizen](https://github.com/commitizen/cz-cli)
- Linters: [commitlint](https://github.com/conventional-changelog/commitlint), [eslint](https://github.com/eslint/eslint), [@antfu/eslint-config](https://github.com/antfu/eslint-config)
- CI/CD: [github actions](https://github.com/features/actions)

## Requirement
  - [node.js](http://nodejs.org/)
  - [volta](https://docs.volta.sh/guide/getting-started)
  - [pnpm](https://pnpm.js.org/en/installation)
  - [encrypted secrets](https://docs.github.com/en/actions/security-guides/encrypted-secrets)

## Getting Started
### GitHub Template

[Create a repo from this template on GitHub](https://github.com/logustra/vivu-npm/generate).

### Clone to local
If you prefer to do it manually with the cleaner git history

```bash
# clone repository
$ git clone https://github.com/logustra/vivu-npm.git

# open folder vivu-npm
$ cd vivu-npm

# install packages
$ pnpm install

# build and serve with vite dev server
$ pnpm dev
```

## Checklist
When you use this template, try follow the checklist to update your info properly

- [ ] Change `name, description, repository, bugs` field in `package.json`
- [ ] Change the author name in `LICENSE`
- [ ] Change the lib name in `vite.config.ts`
- [ ] Change the favicon in `public`
- [ ] Remove the `.github` folder which contains the funding info
- [ ] Clean up the README(s) and remove modules

And, enjoy :)

## Publish to NPM
Make sure you have added the `GIT_TOKEN` and `NPM_TOKEN` encrypted secrets

```bash
# tag git history
$ git tag v0.0.1 -m 'v0.0.1'

# push tag to git
$ git push origin --tags
```

## Usage
### Setup
Vue 3
```js
import { createApp } from 'vue'
import HelloWorld from '@logustra/vivu-npm'
import App from './app.vue'

const app = createApp(App)
app.use(HelloWorld)
```

Vue 2
```js
import Vue from 'vue'
import CompositionAPI from '@vue/composition-api'
import HelloWorld from '@logustra/vivu-npm'

Vue.use(CompositionAPI)
Vue.use(HelloWorld)
```

### Basic Usage
```html
<template>
  <hello-world />
</template>
```
[Demo →](https://codesandbox.io/s/gallant-benji-olf2jh?file=/src/App.vue)

## Cheer me on
If you like my works, you can cheer me on here 😆

&nbsp; &nbsp; 🇮🇩 [Trakteer](https://trakteer.id/logustra/tip)<br>
&nbsp; &nbsp; 🌍 [Ko-Fi](https://ko-fi.com/logustra)<br>

## License
MIT License © 2022 Faizal Andyka