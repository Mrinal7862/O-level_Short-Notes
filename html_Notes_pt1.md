# Notes on HTML Tags

## Headings

- HTML uses `<h1>` to `<h6>` tags to define headings.
  - `<h1>` is the largest heading.
  - `<h6>` is the smallest heading.
- Headings help structure the content on a webpage by creating a clear hierarchy.

### Example:
```html
<h1>This is an h1 heading</h1>
<h2>This is an h2 heading</h2>
<h3>This is an h3 heading</h3>
<h4>This is an h4 heading</h4>
<h5>This is an h5 heading</h5>
<h6>This is an h6 heading</h6>
```
# The output of the given tags
<h1>This is an h1 heading =>  &lth1&gt  </h1>
<h2>This is an h2 heading => &lth2&gt </h2>
<h3>This is an h3 heading => &lth3&gt </h3>
<h4>This is an h4 heading => &lth4&gt </h4>
<h5>This is an h5 heading => &lth5&gt </h5>
<h6>This is an h6 heading => &lth6&gt </h6>

# Paragraph Tag `<p>`

#### HTML uses the `<p>` tag to define paragraphs. Paragraphs are blocks of text that are separated by a blank line in the HTML code. They provide structure and readability to the content.

```html
<p>This is a paragraph.</p>
<p>This is another paragraph.</p>
```

# Lists

### Unordered Lists `<ul>`

#### Unordered lists are defined with the `<ul>` tag. Each item in the list is defined with the `<li>` tag. Items in unordered lists are typically displayed with bullet points.

#### Example:
```html
<ul>
  <li>Item 1</li>
  <li>Item 2</li>
  <li>Item 3</li>
</ul>
```
### Ordered Lists `<ol>`
#### Ordered lists are defined with the `<ol>` tag. Each item in the list is defined with the <li> tag. Items in ordered lists are typically displayed with numbers.

Example:
```html
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>
```
<ol>
  <li>First item</li>
  <li>Second item</li>
  <li>Third item</li>
</ol>

### Nested Lists 


#### Lists can be nested by placing a list inside an `<li>` tag. This can be done with both ordered and unordered lists to create sublists.

Example:
```html
<ul>
  <li>Item 1
    <ul>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ul>
  </li>
  <li>Item 2</li>
</ul>
```
<ul>
  <li>Item 1
    <ul>
      <li>Subitem 1</li>
      <li>Subitem 2</li>
    </ul>
  </li>
  <li>Item 2</li>
    <ol>
        <li>Item 1</li>
        <li>Item 2</li>
        <li>Item 3</li>
    </old>
</ul>