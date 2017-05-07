---
---

## Typography

Bones uses **system fonts**. This means your users get a font that looks good on their devices, and you don't have to load any external resources.

### Headings

<div class="grid">
  <div class="column" markdown="1">
Headings and the content around them have [modular scale](https://alistapart.com/article/more-meaningful-typography) and [vertical rhythm](https://24ways.org/2006/compose-to-a-vertical-rhythm).

Styles are provided for heading levels 1 to 4; you can add your own styles for levels 5 and 6 if you need them.

Heading sizes depend on the `--scale-factor` CSS variable. This controls how much size difference there is between heading levels.

Try changing it:

<input name="scale-factor" id="scale-factor" type="range" min="1" max="2" value="1.4" step="0.1">
  </div>

  <div class="padded center column">
    <h1 style="margin-top: 0;">Apples</h1>
    <h2>Oranges</h2>
    <h3>Peaches</h3>
    <h4>Plums</h4>
  </div>
</div>

## Lists

<div class="grid">
  <div class="column">
    <h3>Unordered</h3>

    <ul>
      <li>flowers</li>
      <li>mouse pad</li>
      <li>bread</li>
      <li>house</li>
    </ul>
  </div>

  <div class="column">
    <h3>Ordered</h3>

    <ol>
      <li>flowers</li>
      <li>mouse pad</li>
      <li>bread</li>
      <li>house</li>
    </ol>
  </div>
</div>


## Tables

Tables have very little style by default, which is a good thing according to [Darkhorse Analytics](http://www.darkhorseanalytics.com/blog/clear-off-the-table).

<table>
  <tr>
    <th>Name</th>
    <th>Occupation</th>
    <th>Age</th>
    <th>Location</th>
  </tr>
  <tr>
    <td>Bernarda Campbell</td>
    <td>ID clerk</td>
    <td>66</td>
    <td>Davenport, IA</td>
  </tr>
  <tr>
    <td>Janice Wrenn</td>
    <td>Conciliator</td>
    <td>40</td>
    <td>Albany, NY</td>
  </tr>
  <tr>
    <td>Francisco Torres</td>
    <td>Builder</td>
    <td>40</td>
    <td>Jackson, OH</td>
  </tr>
</table>


## Buttons

Buttons come in solid, outlined, and clear styles, with different colors for conditional states.

### Styles

<div class="center grid">
  <div class="padded column">
    <h4>Solid</h4>
    <button>Button</button>
  </div>

  <div class="padded column">
    <h4>Outline</h4>
    <button class="outline">Button</button>
  </div>

  <div class="padded column">
    <h4>Clear</h4>
    <button class="clear">Button</button>
  </div>
</div>

``` html
<button>Button</button>

<button class="outline">Button</button>

<button class="clear">Button</button>
```

### States

<div class="center grid">
  <div class="padded column">
    <h4>Primary</h4>
    <button class="primary">Apples</button>
  </div>

  <div class="padded column">
    <h4>Success</h4>
    <button class="success">Oranges</button>
  </div>

  <div class="padded column">
    <h4>Warning</h4>
    <button class="warning">Peaches</button>
  </div>

  <div class="padded column">
    <h4>Danger</h4>
    <button class="danger">Plums</button>
  </div>
</div>

``` html
<button class="primary">Apples</button>

<button class="success">Oranges</button>

<button class="warning">Peaches</button>

<button class="danger">Plums</button>
```


## Forms

Forms have basic, accessible styles.

<form>
  <label>
    Name
    <input type="text" id="name" name="name">
  </label>

  <label>
    Email
    <input type="text" id="email" name="email" required>
  </label>

  <label>
    Age range
    <select>
      <option value="0–10">0–10</option>
      <option value="11–20">11–20</option>
      <option value="21–30">21–30</option>
      <option value="31–40">31–40</option>
      <option value="41–50">41–50</option>
      <option value="50+">50+</option>
    </select>
  </label>

  <label>
    Message
    <textarea id="message" name="message" required></textarea>
  </label>

  <button type="submit">Submit</button>
</form>


## Grid

Bones includes a simple grid based on flexbox, with just a few options.


## Utility classes

Bones includes some helpful utility classes that you can generally add to any element.

### Center

`.center` aligns text inside an element to the center.

### Hide

`.hide` stops an element from being displayed at all.

### Large

`.large` increases an element's size by 20%.

### Small

`.small` decreases an element's size by 20%.
