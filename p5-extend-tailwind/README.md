# Part 5: Extend Tailwind

In this last part, we'll extend Tailwind with some plugins for a blog layout.

## Getting Started

Run the following to install and build CSS for Tailwind:

```bash
$ npm install
$ npm run build
```

This should create a file called `out/compiled.css` that is referenced in the `index.html` file.

## Install Prose plugin

```shell
$ npm install -D @tailwindcss/typography
```

Then add the plugin to your tailwind.config.js file:

```js
// tailwind.config.js
module.exports = {
  theme: {
    // ...
  },
  plugins: [
    require("@tailwindcss/typography"),
    // ...
  ],
};
```

Finally, re-build your CSS file:

```shell
$ npm run build
```
