# CSS Selectors Theory

## What is a Selector?
A selector is a pattern in CSS that is used to select HTML elements so that styles can be applied to them.

Example:

```css
p {
  color: red;
}
```

Here, `p` is the selector and it selects all `<p>` elements.

## Types of Simple Selectors
Simple selectors are used to select elements based on one basic property.

### 1. Tag Name Selector
A tag name selector selects all elements with the same HTML tag.

Example:

```css
p {
  color: blue;
}
```

This selects all `<p>` tags.

### 2. Class Selector
A class selector selects all elements that have the same class name.

Example:

```html
<p class="intro">Hello</p>
<p class="intro">World</p>
```

```css
.intro {
  font-weight: bold;
}
```

The `.` symbol is used before the class name.

### 3. ID Selector
An ID selector selects only one unique element in the document.

Example:

```html
<p id="main">This is a special paragraph.</p>
```

```css
#main {
  color: green;
}
```

The `#` symbol is used before the ID name.

### 4. Grouping Selector
Grouping selectors lets you apply the same style to multiple selectors at once.

Example:

```css
h1, h2, p {
  color: purple;
}
```

This gives the same style to `<h1>`, `<h2>`, and `<p>`.

### 5. Universal Selector
The universal selector selects all elements on the page.

Example:

```css
* {
  margin: 0;
  padding: 0;
}
```

The `*` symbol means all elements.

## Summary
- Selector: A pattern used to target HTML elements.
- Tag name selector: Selects elements by tag name like `p`, `h1`, `div`.
- Class selector: Selects elements by class name using `.`.
- ID selector: Selects one unique element using `#`.
- Grouping selector: Uses commas to style many selectors together.
- Universal selector: Selects every element using `*`.

## Quick Example

```html
<p id="main" class="intro">Hello</p>
<h1>Heading</h1>
<h2>Subheading</h2>
```

```css
* {
  margin: 0;
}

p, h1, h2 {
  color: red;
}

.intro {
  font-size: 20px;
}

#main {
  background-color: yellow;
}
```

This example shows how tag name, class, ID, grouping, and universal selectors work together.