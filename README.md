# chili
Code Highlighter

What is it?
-----------
A small library to highlight code in HTML

Usage
-----
You can import it and add a DOMContentLoaded event to bind to elements that should be highlighted.

```html
<script src="chili.js">
<script>
  window.addEventListener("DOMContentLoaded", () => {
    chili('.highlight');
  });
</script>

<div class="highlight">
  const variable = "Code example";
  console.log(variable);
</div>
```

A compact way using "defer" and "onload" attributes should work as well.

```html
<script src="chili.js" defer onload="chili('.highlight')">
```

Or just embed the code itself with copy/paste instead of load as script.

The library was made to be the simplest and smallest possible to be embeded like this. Is useful for small code examples and documentations.

Languages support
-----------------
The library is language agnostic and should highlight any C based language or the main known programming languages.
Some languages should work better than others.

License
-------
MIT
