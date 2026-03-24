# CSS Position Property

The `position` property in CSS specifies how an element is positioned in the document. It works with the offset properties: `top`, `right`, `bottom`, and `left`.

## Types of Positioning

### 1. static (default)
- Default positioning for all elements.
- Elements follow normal document flow.
- `top`, `left`, etc. have **no effect**.

### 2. relative
- Positioned relative to its **normal position**.
- Can be moved using `top`, `left`, etc.
- Original space is still preserved.

### 3. absolute
- Positioned relative to the **nearest positioned ancestor** (not static).
- If no ancestor exists, it uses the `<html>` element.
- Removed from normal flow (no space reserved).

### 4. fixed
- Positioned relative to the **viewport (browser window)**.
- Does not move when scrolling.
- Removed from normal flow.

### 5. sticky
- Acts like `relative` initially, then like `fixed` when scrolling.
- Sticks to a specified position (e.g., `top: 0`).
- Requires a scrollable container.

## Example

```css
.box {
  position: relative;
  top: 20px;
  left: 10px;
}
````

## Key Points

* `absolute` and `fixed` elements are removed from normal flow.
* `relative` keeps its original space.
* `sticky` depends on scroll behavior.
* Always define at least one offset (`top`, `left`, etc.) for positioning to work.


