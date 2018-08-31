# Iremono

Iremono is a semi-atomic CSS styling kit for designing in code.

## Note well

This is a work in progress. I will be actively updating it in use on current projects. Expect breaking changes.

## How to use it

1. Install: `yarn add callumflack/iremono` or `npm i callumflack/iremono`.

2. Create a variables file. See `variables.example.css` for an example file listing all current css custom properties used in this library. You can customise everything in this library from this file.

3. Then import your `variables.css` and `iremono` it to your CSS imports directory file, as described below. **Note well:** the order of imports matters. Add your variables first, then font-faces (if required), and then `iremono`. Theme stylings should be last. This way, all utilities and mixins within `iremono` will be available in your theme css as well.

```css
/* Variables */
@import "./variables.css";

/* Font faces, if you wish */
@import "./typography/font-face.css";

/* Iremono */
@import "iremono/index.css";

/* Theme your website… */
@import "./theme/button.css";
```

4. Finally, this postcss library makes use of `postcss-mixins`, `postcss-easy-import` and `postcss-preset-env`. Manage their config with a `postcss.config.js` file, an example of which is provided in this repo.

## Documentation

Some form of documentation will be done in time. Suffice to say, no docs at the moment. The best way to check it out is to download it and have a play 🤣. I will, however, list a few techniques:

1. Responsive typography using ems against a body font-size in rems, whose value is updated at media queries.
2. Updating the value of css custom properties in media queries. This means I can manage things like white space responsively with a single line of css that holds a single custom variable. No complicated and tediously managed media queries.
3. The most used utilities are name-spaced with their type's initial letter. For example, width classes start with `w-`. But not every utility is namespaced this way. I don't want to remember too much to use the system.

## What does Iremono mean?

Iremono means "vessel" or "container" in Japanese. I don't speak Japanese, but I came across it serendipitously and I liked how it incorporates the word "mono". I wanted to create a standalone set of CSS patterns I could just drop in to any project. So in my naive dot-connecting way, a "mono vessel" sounded right. The name has stuck for some time.
