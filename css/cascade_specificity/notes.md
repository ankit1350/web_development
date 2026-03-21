
# CSS Cascade and Specificity

## 1. CSS Cascade
The cascade defines how multiple CSS rules are applied to the same element when there are conflicts.

### Cascade Priority Order:
1. **Importance** (`!important`)
2. **Origin**
   - Inline styles
   - Internal/External stylesheets
   - Browser default styles
3. **Specificity**
4. **Source Order** (last rule applied wins)

### Example:
```css
p { color: blue; }
p { color: red; }
````

➡️ Output: `red` (last rule wins)

---

## 2. CSS Specificity

Specificity determines which CSS rule is applied when multiple rules target the same element.

### Specificity Hierarchy:

| Selector Type                | Value |
| ---------------------------- | ----- |
| Inline styles                | 1000  |
| ID selectors                 | 100   |
| Class/Attribute/Pseudo-class | 10    |
| Element/Pseudo-element       | 1     |

### Example:

```css
#id { color: red; }      /* 100 */
.class { color: blue; }  /* 10 */
p { color: green; }      /* 1 */
```

➡️ Output: `red` (highest specificity)

---

## 3. Important Notes

* `!important` overrides all normal rules.
* More specific selector > less specific selector.
* If specificity is equal, **last declared rule wins**.
* Inline styles have highest priority (except `!important`).

---

* Cascade = *order of applying styles*
* Specificity = *priority of selectors*
* Rule applied = highest specificity OR last rule (if equal)

```

