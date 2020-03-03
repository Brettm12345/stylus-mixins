# Stylus Mixins

A collection of shorthand mixins for [stylus-lang](https://stylus-lang.com/)

## Usage

```sh
yarn add -D stylus-mixins
```

```css
@import "stylus-mixins";
```

## Mixins

### [Border](lib/_border.styl)

| Mixin | Property                       |
| ----- | ------------------------------ |
| `b`   | `border`                       |
| `bt`  | `border-top`                   |
| `bl`  | `border-left`                  |
| `br`  | `border-right`                 |
| `by`  | `border-top` & `border-bottom` |
| `bx`  | `border-left` & `border-right` |
| `r`   | `border-radius`                |

### [Colors](lib/_colors.styl)

#### The `c` mixin

The `c` mixin works like this

```css
// c <color> <border-color> <background-color> <color-important> <border-color-important> <background-color-important>
```

```scss
input
  c white gray black 1 0 1
```

would expand to

```css
input {
  color: white !important;
  border-color: gray;
  background-color: black !important;
}
```

> note you can use `0` to omit arguments

| Mixin | Property     |
| ----- | ------------ |
| `c`   | see below    |
| `bg`  | `background` |
| `fg`  | `color`      |

### [Misc](lib/_misc.styl)

| Mixin | Property     |
| ----- | ------------ |
| `an`  | `animation`  |
| `d`   | `display`    |
| `bs`  | `box-shadow` |
| `tr`  | `transition` |
| `op`  | `opacity`    |

### [Spacing](lib/_spacing.styl)

| Mixin | Property                         |
| ----- | -------------------------------- |
| `p`   | `padding`                        |
| `pb`  | `padding-bottom`                 |
| `pl`  | `padding-left`                   |
| `pr`  | `padding-right`                  |
| `px`  | `padding-left` & `padding-right` |
| `py`  | `padding-top` & `padding-bottom` |
| `m`   | `margin`                         |
| `mb`  | `margin-bottom`                  |
| `ml`  | `margin-left`                    |
| `mr`  | `margin-right`                   |
| `mx`  | `margin-left` & `margin-right`   |
| `my`  | `margin-top` & `margin-bottom`   |

### [Typography](lib/_typography.styl)

| Mixin | Property          |
| ----- | ----------------- |
| `ff`  | `font-family`     |
| `fs`  | `font-size`       |
| `fw`  | `font-weight`     |
| `td`  | `text-decoration` |

### Todo

[ ] - Add tests
