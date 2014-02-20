*This repository is a mirror of the [component](http://component.io) module [yields/carry](http://github.com/yields/carry). It has been modified to work with NPM+Browserify. You can install it using the command `npm install npmcomponent/yields-carry`. Please do not open issues or send pull requests against this repo. If you have issues with this repo, report it to [npmcomponent](https://github.com/airportyh/npmcomponent).*

# carry

  Carry attrs, classes from one element to another.

## Installation

  Install with [component(1)](http://component.io):

    $ component install yields/carry

## Example

```js

function Widget(el){
  this.el = carry(el, tpl.cloneNode());
}

new Widget;
new Widget(el);

```

## API

#### carry(a, b)

  if `a` is `null` a clone of `b` will be returned.
  otherwise `b`'s attrs and classes are merged with `a`,
  returning `a`.

#### .attrs(a, b)

Carry over attributes from `b` to `a`.

#### .classes(a, b)

Carry over classes from `b` to `a`.

## License

  MIT
