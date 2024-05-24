# Unocss preset pico

An preset to ease the usage of [Pico css](https://picocss.com/) with [Unocss](https://unocss.dev/).

It adds all Pico css colors the theme, so you can use it in classes:

```html
<p text-pico-primary>Hello pico!!</p>
```

Will generate the css class:

```css
.text-pico-primary {
  color: var(--pico-primary);
}
```

See All the Pico css variables on the [documentation website](https://picocss.com/docs/css-variables#all-css-variables).

## Installation:

```sh
npm install -D unocss-preset-pico
```

## Configuration

Add the preset to your unocss.config.ts file:

```ts
import { defineConfig, presetUno } from "unocss";
import presetPico from "unocss-preset-pico";

export default defineConfig({
  presets: [presetUno(), presetPico()],
});
```
