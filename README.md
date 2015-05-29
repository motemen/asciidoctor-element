asciidoctor-element
===================

Element wrapper for the [asciidoctor.js](https://github.com/asciidoctor/asciidoctor.js) library.

`<asciidoctor-element>` accepts AsciiDoc source either via its `asciidoc` attribute:

```html
<asciidoctor-element asciidoc="`AsciiDoc` is _awesome_!"></asciidoctor-element>
```

Or, you can provide it via a `<script type="text/asciidoc">` element child:

```html
<asciidoctor-element>
  <script type="text/asciidoc">
    Check out my asciidoc!

    We can even embed elements without fear of the HTML parser mucking up their
    textual representation:

    <awesome-sauce>
      <div>Oops, I'm about to forget to close this div.
    </awesome-sauce>
    
  </script>
</asciidoctor-element>
```

Note that the `<script type="text/asciidoc">` approach is _static_. Changes to
the script content will _not_ update the rendered asciidoc!
