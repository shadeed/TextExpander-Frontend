# TextExpander-Frontend
Text Expander Snippets for Front-End Developers

## Form Input

Snippet:

```html
<input type="%filltext:name=Type%" id="%filltext:name=ID%" 
class="%filltext:name=Class%" %fillpart:name=ARIA Required:default=yes%aria-required="true"%fillpartend%>
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




