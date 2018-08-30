# Iremono

Iremono is a semi-atomic CSS styling kit for designing in code.

## How to use it

Install: `yarn add` or `npm i`

Then add it to your CSS imports directory file, like so:

```
/* Variables */
@import "./variables.css";

/* Typography */
@import "./typography/font-face.css";

/* Iremono */
@import "iremono/index.css";

/* Theme */
@import "./theme/button.css";
```

Notice the variables file. Customise everything from there. An example with every variable in this library is included. See `variables.example.css`.

Finally, this postcss library makes use of `postcss-mixins`, `postcss-easy-import` and `postcss-preset-env`. I like managing their config with a `postcss.config.js` file, an example of which is provided.

## WHat the hell does Iremono mean?

Iremono means "vessel" or "container" in Japanese. I don't speak Japanese, but I like how it incorporates "mono". I wanted a standalone set of CSS patterns I could just drop in to any project.
