# sizing units:-

* viewport = takes the fraction height or width of the device
    * 100vw = occupies 100% widht of the device
    * 50vh =  occupies 50% height of the device

* margin:auto 
    - equal spaces from left and right . i.e in center
    - not applied to inline elements
    * if margin=23px auto:
        - auto from left right and 23px margin from top and bottom.

* em :-
    * font-size: 1.2em; it means 1.2 times of (`element`) wtv the font size applied to it.

* rem :-
    * font-size: 1.2rem; it means 1.2 times of the `root element`
* vmin or vmax :-
    * in laptop : vmin is the height and vmax is the width
    * in mobile : vmin is the width and vmax is the height
    used for responsive designs based on the compatibility of the device.

CSS sizing units define the size of elements like width, height, margin, padding, and font-size.

---

## 1. Absolute Units
Fixed size units that do not change based on screen or parent.

| Unit | Description |
|------|------------|
| px   | Pixels (most commonly used) |
| cm   | Centimeters |
| mm   | Millimeters |
| in   | Inches |
| pt   | Points (1pt = 1/72 inch) |
| pc   | Picas (1pc = 12pt) |


---

## 2. Relative Units

Depend on parent element or viewport size.

### a) Font-relative Units

| Unit | Description                       |
| ---- | --------------------------------- |
| em   | Relative to parent font-size      |
| rem  | Relative to root (html) font-size |

---

### b) Viewport Units

| Unit | Description           |
| ---- | --------------------- |
| vw   | 1% of viewport width  |
| vh   | 1% of viewport height |
| vmin | Smaller of vw or vh   |
| vmax | Larger of vw or vh    |

---

### c) Percentage (%)

* Relative to parent element size.(inherits the property applied to its parents ans applies % to it.)

---

## 3. Key Points

* `px` is fixed → not responsive.
* `em` can cause compounding issues.
* `rem` is preferred for consistent scaling.
* `vw` and `vh` are useful for responsive layouts.
* `%` depends on parent size.

---

* Absolute = fixed (px, cm, etc.)
* Relative = flexible (em, rem, %, vw, vh)
* Use `rem`, `%`, and `vw/vh` for responsive design

```