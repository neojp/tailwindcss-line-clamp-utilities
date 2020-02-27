<p align="center">
    <a href="https://tailwindcss.com/" target="_blank"><img width="200" src="https://tailwindcss.com/img/tailwind.svg"></a><br>
    A utility-first CSS framework for rapidly building custom user interfaces.
</p>

---

<br>

# Tailwind CSS `line-clamp` utilities

This is a Tailwind CSS plugin that adds utilities to restrict the amount of lines an element can have by using the CSS property [line-clamp](https://css-tricks.com/almanac/properties/l/line-clamp/).

Maintained by: [Joan Piedra](https://joanpiedra.com) → [@neojp](https://twitter.com/neojp)

## Installation

Install as a node module with either `npm` or `yarn` on your command line

```bash
# Install via npm
npm install --save-dev @neojp/tailwindcss-line-clamp-utilities

# Install via yarn
yarn add --dev @neojp/tailwindcss-line-clamp-utilities
```

Add this module as a plugin on your [Tailwind configuration file](https://tailwindcss.com/docs/configuration#plugins) (`tailwind.config.js`).

```js
module.exports = {
  plugins: [
      require('@neojp/tailwindcss-line-clamp-utilities')
  ]
};
```

### Variants

Note that this plugin allows the usage of variants through the key `lineClamp` and will default to your global variant setting.

```js
module.exports = {
  variants: {
    lineClamp: ['responsive']
  }
};
```


## Usage

Use the Tailwind utility classes provided by this plugin.

```html

<div class="line-clamp-1"></div>
<div class="line-clamp-2"></div>
<div class="line-clamp-3"></div>
<div class="line-clamp-4"></div>
<div class="line-clamp-5"></div>
<div class="line-clamp-6"></div>
<div class="line-clamp-7"></div>
<div class="line-clamp-8"></div>
<div class="line-clamp-9"></div>
<div class="line-clamp-10"></div>

```

### Examples

Restrict content to 3 lines:

```html
<div class="line-clamp-3 w-64">
  <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Nulla pulvinar, dui vel viverra aliquet, sem nulla sollicitudin diam, et dapibus lectus neque vitae risus. Sed elit risus, facilisis in condimentum quis, luctus ac leo. Integer viverra vel orci quis accumsan. Etiam vitae elementum orci. Sed non venenatis lorem. Pellentesque a metus varius sapien finibus euismod ac et arcu. Donec eu nisl a sem pulvinar tristique in at massa.</p>
</div>
```

Will be displayed as:

```
Lorem ipsum dolor sit amet,
consectetur adipiscing elit. Nulla
pulvinar, dui vel viverra aliquet, se...
```

## Output

Tailwind will be outputed as follows.

```css
.line-clamp-1 {
  display: -webkit-box;
  -webkit-line-clamp: 1;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-2 {
  display: -webkit-box;
  -webkit-line-clamp: 2;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-3 {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-4 {
  display: -webkit-box;
  -webkit-line-clamp: 4;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-5 {
  display: -webkit-box;
  -webkit-line-clamp: 5;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-6 {
  display: -webkit-box;
  -webkit-line-clamp: 6;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-7 {
  display: -webkit-box;
  -webkit-line-clamp: 7;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-8 {
  display: -webkit-box;
  -webkit-line-clamp: 8;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-9 {
  display: -webkit-box;
  -webkit-line-clamp: 9;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

.line-clamp-10 {
  display: -webkit-box;
  -webkit-line-clamp: 10;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
```

## Related plugins

Shout out to [tailwindcss-aspect-ratio](https://github.com/webdna/tailwindcss-aspect-ratio) another plugin that attemps to handle aspect ratios on Tailwind CSS.

## Contributing

Feel free to submit a PR request, and send me a message on Twitter ([@neojp](https://twitter.com/neojp)) about it.

## License
This project has been licensed under [the Hippocratic License](https://firstdonoharm.dev/).