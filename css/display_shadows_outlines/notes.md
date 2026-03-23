# CSS Short Notes

## 1. CSS Display
The `display` property defines how an element is rendered in the layout.

### Common Values:
- `block` → Takes full width, starts on a new line (e.g., `<div>`)
- `inline` → Takes only necessary width, no line break (e.g., `<span>`)
- `inline-block` → Inline but allows width/height
- `none` → Hides the element (removes from layout)
- `flex` → Enables flexbox layout
- `grid` → Enables grid layout

---

## 2. CSS Shadows

### (a) Box Shadow
Adds shadow around elements.

**Syntax:**
```

box-shadow: h-offset v-offset blur spread color;
*  if `inset` is used, then the shadow will be formed inside the box.
```

**Example:**
```

box-shadow: 2px 2px 5px gray;

```

### (b) Text Shadow
Adds shadow to text.

**Syntax:**
```

text-shadow: h-offset v-offset blur color;

```

**Example:**
```

text-shadow: 1px 1px 3px black;

```

---

## 3. CSS Outline
The `outline` property draws a line outside the border.

### Properties:
- `outline-width`
- `outline-style`
- `outline-color`

outline: 2px solid red;

```

### Key Points:
- Does not take space (unlike border)
- Used for focus and accessibility
---

## 4. CSS Overflow
Controls what happens when content exceeds container size.

### Values:
- `visible` → Default, content spills out
- `hidden` → Extra content is clipped
- `scroll` → Adds scrollbars
- `auto` → Scrollbars appear only if needed

**Example:**
```

overflow: auto;

```

---

## Summary
- `display` controls layout behavior
- `shadows` enhance visual appearance
- `outline` highlights elements without affecting layout
- `overflow` manages excess content
```
