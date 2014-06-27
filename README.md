# Globant HTML Style Guide() {

*A mostly reasonable approach to HTML*


## <a name='TOC'>Table of Contents</a>

#Work in progress.

### HTML quotation marks
When quoting attributes values, use double quotation marks. Use double ("") rather than single quotation marks ('') around attribute values.


```
  <!-- bad -->
  <a class='maia-button maia-button-secondary'>Sign in</a>

  <!-- good -->
  <a class="maia-button maia-button-secondary">Sign in</a>
```

### Name your content by HTML structural elements.
Never name your content after the visual appearance but after its description. (e.g. prefer "sidebar-container" than "left-container")

```
  <body>
    <div id="container">
      <div id="header-container">
        <div class="logo">...</div>
        <div>...</div>
      </div>
      <div id="content-container">...</div>
      <div id="sidebar-container">...</div>
    </div>
  </body>
```

### White Space
Indent using soft tabs set to 2 spaces, don't use hard tabs.

```
  <div class="container">
  ∙∙<h1>Header</h1>
  </div>
```


### HTML Attributes Naming
Name your id & classes after the elements description and not about the visual elements, use `.external-link` instead of `.red-link` => what if you change the color of the link?
Use hyphen to name your attributes and class.

```
	<div>
    <div id="header-container">
      <div id="header-title" class="title">...</div>
    </div>
	</div>
```

### Doc Type:
Ensure that all websites use the new HTML5 doctype

```
  <!doctype html>
```

### alt:
All images which are using the <img> tag should use the alt attribute. If not alternative is provided, it is still mandatory to use the alt attribute but with an empty string to comply with accessibility rules.

### Meta Tags:
#### Character set
Ensure that all websites use UTF-8 character sets so that the pages can be read universally

```
  <meta charset="utf-8">
```
#### Mobile / Responsive
Make sure to include a viewport meta tag when building a responsive or mobile dedicated website
<https://developer.mozilla.org/en-US/docs/Mobile/Viewport_meta_tag>

```
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
```

}
=
