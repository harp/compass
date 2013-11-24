# harp-compass

> Core mixins from Compass, the Sass-based stylesheet authoring environment.

## Dependencies

* [NodeJS](http://nodejs.org/) – _Server-side JavaScript runtime_
* [Harp](http://harpjs.com/) – _The static web server with built-in preprocessing_

## Resources

* [Harp documentation](http://harpjs.com/docs)
* [Sass documentation](http://sass-lang.com/documentation/file.SASS_REFERENCE.html)
* [Compass documentation](http://compass-style.org/reference/compass/)

## Install

To install Compass Core, run the following command from the root of your harp project:

```bash
harp install compass
```

Your project will look something like this…

```
myproject/                  <-- your project root (or public dir if in framework-mode)
  |- components/            <-- harp puts components here
  |   +- harp-compass/         <-- where this lib is installed
  |       …
  |- main.scss              <-- where you reference Compass Core 
  +- index.jade             <-- where you reference main.css
```

## Link

Now, from within an `.scss` file in your project, you can `@import` Compass:

```scss
@import "components/harp-compass/scss/compass";
```

By default, Compass Core doesn’t include the Layout or Reset modules. You may choose import those, too:

```scss
@import "components/harp-compass/scss/reset";
@import "components/harp-compass/scss/compass";
@import "components/harp-compass/scss/layout";
```

Or, simply import a portion of Compass:

```scss
@import "components/harp-compass/scss/css3";
```

## License

This component is [Compass](https://github.com/chriseppstein/compass), which is Copyright © 2008-2009 Christopher M. Eppstein and MIT licensed.