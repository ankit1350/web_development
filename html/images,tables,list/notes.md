# HTML Images, Videos & Tables

## 1. Images (`<img>` tag)

### Basic syntax

```html
<img src="pic1.png" alt="description">
```

### Keeping aspect ratio (IMPORTANT)

To maintain the **original aspect ratio** of an image:

* **Change only ONE attribute** → either `width` **or** `height`

✅ Correct examples:

```html
<img src="pic1.png" width="400" alt="sample image">
<img src="pic1.png" height="300" alt="sample image">
```

❌ Wrong example (distorts image):

```html
<img src="pic1.png" width="400" height="300">
```

### Useful attributes

* `src` → path of image
* `alt` → alternative text (SEO + accessibility)
* `width` / `height` → size control
* `loading="lazy"` → improves performance

```html
<img src="pic1.png" width="400" alt="image" loading="lazy">
```

---

## 2. Videos (`<video>` tag)

### Basic syntax

```html
<video controls>
  <source src="vid1.mp4" type="video/mp4">
</video>
```

### Keeping aspect ratio (IMPORTANT)

Same rule as images:

* Modify **only width OR height**, not both

✅ Correct:

```html
<video width="600" controls>
  <source src="vid1.mp4" type="video/mp4">
</video>
```

❌ Wrong:

```html
<video width="600" height="300"></video>
```

### Common video attributes

* `controls` → play / pause buttons
* `autoplay` → auto play (needs `muted`)
* `muted` → mute audio
* `loop` → repeat video

```html
<video width="500" controls autoplay muted loop>
```

---

## 3. HTML Tables

### Basic structure

Every table has:

* `<table>` → the table itself
* `<tr>` → table row
* `<th>` → table heading
* `<td>` → table data (cell)

### Example

```html
<table border="1">
  <tr>
    <th>Name</th>
    <th>Age</th>
  </tr>
  <tr>
    <td>Ankit</td>
    <td>20</td>
  </tr>
</table>
```

---



---

## 5. Merging Cells

### `colspan` (merge columns)

```html
<td colspan="2">Merged Column</td>
```

### `rowspan` (merge rows)

```html
<td rowspan="2">Merged Row</td>
```

⚠️ Rule: Total columns must remain consistent.

---

## 6. Styling Tables with CSS (Recommended)

```css
table {
  border-collapse: collapse;
  width: 100%;
}

th, td {
  border: 1px solid black;
  padding: 8px;
  text-align: center;
}
```

---

## 7. Accessibility Tips (Important)

```html
<th scope="col">Name</th>
<th scope="row">Total</th>
```

* Helps screen readers
* Improves SEO

---

 Summary

* Use `<img>` and `<video>` carefully
* Modify only one dimension
* Tables have strict structure
* Markdown helps in clean documentation
