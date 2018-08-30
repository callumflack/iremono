# Iremono

Iremono is a semi-atomic CSS styling kit for designing in code.

## Note well

This is a work in progress. I will be actively updating it in use on current projects. Expect heavy, breaking changes.

## How to use it

1. Install: `yarn add` or `npm i`

2. Create a variables file. You can customise everything pattern in the library there. See `variables.example.css` for an example file listing all current variables (aka css custom properties).

3. Then import your `variables.css` and `iremono` it to your CSS imports directory file, as described below.

**Please note well:** the order of imports matters. Add your variables first, then font-faces (if required), then `iremono`. Theme stylings should be last.

```css
/* Variables */
@import "./variables.css";

/* Font faces, if you wish */
@import "./typography/font-face.css";

/* Iremono */
@import "iremono/index.css";

/* Theme it how ever you wish */
@import "./theme/button.css";
```

4. Finally, this postcss library makes use of `postcss-mixins`, `postcss-easy-import` and `postcss-preset-env`. I like managing their config with a `postcss.config.js` file, an example of which is provided.

## What does Iremono mean?

Iremono means "vessel" or "container" in Japanese. I don't speak Japanese, but I cam across it serendipitously and I liked how it incorporates the word "mono". I wanted to create a standalone set of CSS patterns I could just drop in to any project. The name has stuck for some time.
