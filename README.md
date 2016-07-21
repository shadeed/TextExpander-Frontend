# TextExpander-Frontend
[Text Expander](https://textexpander.com) Snippets for Front-End Developers

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

## Vertical Spacing Between Elements

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