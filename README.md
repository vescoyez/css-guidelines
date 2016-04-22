# CSS Guidelines (under construction)

## Single responsability

The single responsibility principle states that every module or chunk of code (a function etc) should do one job well and one job only. The benefits of this are mainly in the way of maintainability and extensibility.

### Responsabilities

#### Base

- `display`

#### Structural

- `margin`
- `padding`

#### Cosmetic

- `color`
- `font-family`
- `background-color`
- `font-size`
- `line-height`
- `font-weight`
- `letter-spacing`
- `text-transform`
- `text-underline`

## Typography

### General

Style the `h1` to `h6`, `p` and `ul`/`ol` as they look good in a text without any class. As a WYSIWYG could output it.

That includes:
- `font-family`
- `font-size`
- `line-height`
- `margin` (in `em`)
- `font-color`
- `letter spacing` (in `em`)

### Custom Titles

Reset the margin on all custom title

###### Example
```css
.title {
  margin: 0;
}
```

Add cosmetic variant you need (no `margin`)

###### Example
```css
.title--1 {
  font-size: 20px;
  color: #636974;
  line-height: 1.4;
}
.title--2 {
  font-size: 16px;
  color: #333;
}
```

Add the structure depending of the context

###### Example

```css
.card__title {
  margin: 12px 0;
}
```

HTML result:

```html
<h2 class="card__title title title--1">Card Title</h2>
```
