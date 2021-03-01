# Part 3: Install using PostCSS

## Getting Started

Run the following to install and build CSS for Tailwind:

```bash
$ npm install
$ npm run build
```

This should create a file called `out/compiled.css` that is referenced in the `index.html` file.

## What dependencies are we using?

In this example, we've set up a Node project with the following developer dependencies:

- `postcss`: allows us to compile and use modern/experimental CSS syntax
- `postcss-cli`: CLI for PostCSS (used for building final CSS file)
- `tailwindcss`: PostCSS plugin used to install Tailwind
- `autoprefixer`: PostCSS plugin used to provide consistent styling across browsers

## What are all these files for?

- `package.json`: Let's us define what packages to pull from NPM
- `package-lock.json`: Works in tandem with `package.json` to ensure all developers using this project get the same version of dependencies
- `postcss.config.js`: Configure PostCSS to add Tailwind and Autoprefixer plugins
- `styles.css`: Base CSS file that tells PostCSS which Tailwind utility classes to include
- `tailwind.config.js`: Configure & extend Tailwind to support different features and optimize final CSS file
