* if Radio tag is used : then only one option can be selected at most
```html
<label for="age">18 years or above?</label>
```
* ## if the id does not match then marking can be done only on the circle
  * if the id is correct then the marking can **also** be done by just clicking the label written over there

* **Get** request is used for simple data ~ *limited*
    * passwords

* **Post** request is used for large data sets
* autofocus:focuses the cursor automatically when the page loads
```html
<option value="In">India</option>  
```

*   ** user sees India and the servers receives In **

Sure 👍
Here are **SHORT NOTES** based on the topics we discussed (perfect for revision / exams).

---

### 1️ `name` Attribute

* Used to **identify form data**
* Data is sent as `name=value` pair
* **Mandatory** for backend processing



### 2 `value` Attribute

* Stores the **actual data sent to server**
* Backend only reads `value`, not label text

### 3️ `id` Attribute

* Used for **CSS, JavaScript, and label linking**
* Must be **unique**
* Not sent to server

### 4️ `label` Tag

* Improves **accessibility**
* **Clicking label focuses input**
* Connected using `for=id`


### 5️ Radio Button

* Used to select **only one option**
* Same `name` groups radios


### 6️ Checkbox

* Used for **multiple or yes/no choices**
* If unchecked → data not sent
* Without value → sends `on` (bad practice)
-
### 7️`textarea`

* Used for **multi-line input**  ~description...
* Text inside is actual value

---
### 8️ `select` & `option`

* Dropdown menu
* `value` is sent to server, text is shown to user
---

### 9️ `form` Attributes

* `action` → where data goes
* `method` → how data is sent (`GET` / `POST`)
---

### 🔑 Golden Rule (Very Important)

> **`name` = key, `value` = data, `id` = identifier**

