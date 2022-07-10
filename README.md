# Vite-React-Typescript-Sass-Bootstrap-Starter

A vite+react+typescript+sass+bootstrap starter

## Easy start

```bash
gh repo clone calidion/Vite-React-Typescript-Sass-Bootstrap-Starter {your-project-name}
cd {your-project-name}
yarn
yarn dev
```

## Step By Step Setup

### Create a vite + bootstrap + typescript project with vite built in tool

```bash
yarn create vite
```

then you should fill in your project name with prompt:

```bash
? Project name: › vite-project
```

after filled in your project name, you should choose the framework you would like to use with prompt like this:

```bash
? Select a framework: › - Use arrow-keys. Return to submit.
❯   vanilla
    vue
    react
    preact
    lit
    svelte
```

here we choose `react` and more specifically `react-ts` as we will see the following variants selection section after `react` chosen.

```bash
? Select a variant: › - Use arrow-keys. Return to submit.
❯   react
    react-ts
```

Now we have a react + typescript project ready.

Then we start to add support for
bootstrap and sass.

### Install bootstrap

Add dependency to `package.json`

```bash
yarn add bootstrap
yarn add @popperjs/core
```

### Install node.js types

```bash
yarn add --dev @types/node
```

### Install sass support

```bash
yarn add sass
```

### Change `.css` files to `.scss`

Change `index.css` to `index.scss`
Change `App.css` to `App.scss`

### Change `.css` imports to `.scss`

#### Change `main.tsx`

```ts
import './index.css'
```

to

```ts
import './index.scss'
```

#### Change `App.tsx`

```ts
import './App.css'
```

to

```ts
import './App.scss'
```

### Import Bootstrap JS when needed

```ts
import { Tooltip, Toast, Popover } from 'bootstrap';
```

Normally you don't need import bootstrap package. But when you need `Tooltip`, `Toast`, `Popover` to work properly, you need to import them into your react components.
