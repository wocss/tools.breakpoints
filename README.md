# Breakpoints

> Tool

The `wocss-tools-breakpoints` module contains simple media queries `mixins`.

Install using npm:

```sh
$ npm install wocss-tools-breakpoints --save
```

## Usage

With a tool like [webpack](https://webpack.github.io/) you can import this module writing:

```scss
// dependencies imports

@import '~wocss-tools-breakpoints';
```

### Mixins

Then you can use these mixins:

#### from($size)

Styles take effect from the provided measure and above.

```scss
@include from('lg') { ... }
```

#### to($size)

Styles take effect from zero up to the provided measure.

```scss
@include to('md') { ... }
```

#### from-to($desde, $hasta)

When the screen size is between the two provided measure, the styles in the block will take effect.

```scss
@include from-to(500px, 800px) { ... }
```

## Dependencies

* [wocss-settings-breakpoints](https://github.com/wocss/settings.breakpoints)
