# TextExpander-Frontend
[Text Expander](https://textexpander.com) Snippets for Front-End Developers

Please feel free to contribute and add any snippet you want, also if you see that something should be better, do not hesitate to create a pull request.

## Form Input

Snippet:

```html
<label for="%filltext:name=ID%"></label>%key:enter%
<input type="%filltext:name=Type%" id="%filltext:name=ID%" class="%filltext:name=Class%" %fillpart:name=ARIA Required:default=yes%aria-required="true"%fillpartend%>
```

Attributes:
- type
- ID
- class
- aria-required

Expanded Result:

```html
<label for="email"></label>
<input type="email" id="email" class="form-input" aria-required="true"> 
```

## SVG Icon

Snippet:

```html
<svg width="%filltext:name=Width%" height="%filltext:name=Height%" viewBox="0 0 32 32">
       <use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#%filltext:name=Icon ID%"></use>
</svg>
```

Attributes:
- width
- height
- icon id

Expanded Result:

```html
<svg width="32" height="32" viewBox="0 0 32 32">
       <use xmlns:xlink="http://www.w3.org/1999/xlink" xlink:href="#icon-github"></use>
</svg>
```

## Article Element

Snippet:

```html
<article>
  <header>
        
  </header>

  <footer>
        
  </footer>
</article>
```

Expanded Result:
No need.

## HTML Fieldset

Snippet:

```html
<fieldset>
    <legend>%filltext:name=Legend%</legend>
</fieldset>
```

Expanded Result:

```html
<fieldset>
    <legend>Title</legend>
</fieldset>
```

## Container

Snippet:

```css
.foo {
    max-width: %filltext:name=Max width%;
    margin-left: auto;
    margin-right: auto;
    padding-left: %filltext:name=Padding%;
    padding-right: %filltext:name=Padding%;
}
```

Expanded result:

```css
.foo {
    max-width: 60em;
    margin-left: auto;
    margin-right: auto;
    padding-left: 1em;
    padding-right: 1em
}
```

## Vertical Spacing

Snippet:

```css
.foo {
    margin-%fillpopup:name=Select margin direction:default=top:bottom%: %filltext:name=Value%;
}
```

Expanded result:

```css
.foo {
    margin-top: 20px;
}
```

or

```css
.foo {
    margin-bottom: 20px;
}
```

## Horizontal Spacing

Snippet:

```css
.foo {
    margin-%fillpopup:name=Select margin direction:default=left:right%: %filltext:name=Value%;
}
```

Expanded result:

```css
.foo {
    margin-right: 20px;
}
```

or

```css
.foo {
    margin-left: 20px;
}
```

## Image `src`

Snippet:

```html
<div class="image-wrapper">
  <img src="%clipboard" alt="%filltext:default=image%">
</div>
```

Copy image source and then type the abbreviaiton, TextExpander will popup and let you add the `alt` text content.

Expanded result:

```html
<div class="image-wrapper">
  <img src="path/to/image" alt="Image">
</div>
```

Snipper [Source](http://code.tutsplus.com/articles/textexpander-for-web-developers--net-26402)


## Placeholder Images

Snippet:

```html
<img src="http://placehold.it/%filltext:name=Width:default=100%x%filltext:name=Height:default=100%">
```

Expanded result:

```html
<img src="http://placehold.it/100x100">
```

