## Colors

<style>
  .color-list {
    list-style-type: none;
  }

  .swatch {
    display: inline-block;
    width:  var(--space-half);
    height: var(--space-half);
    background: var(--color-bg);
    border: 1px solid var(--color-bg);
    border-radius: 50%;
    vertical-align: middle;
  }
</style>

Most colors are approximately taken from [Material Design](https://www.materialui.co/colors). State colors are used to describe different _states_ (like "success", "warning", or "danger"), and by default are mapped to one of the primary colors.

<div class="grid">
  <div class="column">
    <ul class="color-list">
      <li><span class="swatch" style="background: var(--color-red)"></span> red / danger</li>
      <li><span class="swatch" style="background: var(--color-pink)"></span> pink</li>
      <li><span class="swatch" style="background: var(--color-purple)"></span> purple</li>
      <li><span class="swatch" style="background: var(--color-indigo)"></span> indigo</li>
      <li><span class="swatch" style="background: var(--color-blue)"></span> blue / primary</li>
      <li><span class="swatch" style="background: var(--color-cyan)"></span> cyan</li>
    </ul>
  </div>
  <div class="column">
    <ul class="color-list">
      <li><span class="swatch" style="background: var(--color-teal)"></span> teal</li>
      <li><span class="swatch" style="background: var(--color-green)"></span> green / success</li>
      <li><span class="swatch" style="background: var(--color-lime)"></span> lime</li>
      <li><span class="swatch" style="background: var(--color-yellow)"></span> yellow</li>
      <li><span class="swatch" style="background: var(--color-orange)"></span> orange / warning</li>
      <li><span class="swatch" style="background: var(--color-brown)"></span> brown</li>
    </ul>
  </div>
  <div class="column">
    <ul class="color-list">
      <li><span class="swatch" style="background: var(--color-black)"></span> black</li>
      <li><span class="swatch" style="background: var(--color-grey)"></span> grey / subdued</li>
      <li><span class="swatch" style="background: var(--color-light)"></span> light / bg</li>
      <li><span class="swatch" style="background: var(--color-white)"></span> white</li>
    </ul>
  </div>
</div>

You can remap a state color to a different primary color by reassigning its variable in the `:root` selector:

``` css
  :root {
    --color-primary: var(--color-purple);
  }
```
