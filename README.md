# Convert CSS Starter to Tailwind Starter POC

To convert, run:

```
npm run convert-to-tailwind
```

Uses https://www.npmjs.com/package/css-modules-to-tailwind behind the scenes.

## Misc Notes

- Project created with create pantheon-decoupled-kit
- Tailwind added by create pantheon-decoupled-kit
- Tailwind config file added by create pantheon-decoupled-kit
  - Possible bug for this use case: globals.css was reset to include only tailwind imports. Currently we need to merge the two files.
- After converting, you'll mostly note that not as much of the css modules were converted as you'd expect. css-modules-to-tailwind leaves the things it doesn't understand untouched. In this case it is mostly css variables. We'd have to restructure our css a bit to take advantage of this approach.