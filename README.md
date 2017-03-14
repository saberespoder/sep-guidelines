# sep-guidelines npm package

This package based on UX/UI guidelines for Saberespoder services. The main foundation of this package is [Twitter Bootstrap v.3.3](http://getbootstrap.com/) styled according to sep guidelines. Further changes should be applied by tweking [variables file](src/_variables.less)

## Rebuild package

In the most cases we would need to include built files from the `sep-guidelines/build` directory. Basically, there are two approaches to get files updated there:

1. Say `npm run build`
2. Run package publishing by `npm publish ./` This command will publish npm package on [npmjs.com](https://www.npmjs.com/package/sep-guidelines) and consequently prebuild assets (thanks to *prepublish* section in [package.json](package.json))

## Include package

Since we intended to use this package mostly in our Ruby-based projects the easies way to include files will look like so:

**Stylesheets**

```sass
@import "sep-guidelines/build/index";
```

**JavaScripts**

```javascript
//= require "sep-guidelines/build/index"
```
