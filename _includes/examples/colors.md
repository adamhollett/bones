## Colors

<style>
  .color-list {
    list-style-type: none;
    margin-bottom: 0;
  }

  .swatch {
    display: inline-block;
    width:  2rem;
    height: 2rem;
    margin-right: 1rem;
    background: var(--color-bg);
    border: 1px solid var(--color-bg);
    border-radius: 50%;
    vertical-align: middle;
  }
</style>

Most colors are approximated from [Material Design](https://www.materialui.co/colors). State colors are used to describe different _states_ (like "success", "warning", or "danger"), and by default are mapped to one of the primary colors.

Colors are implemented using native CSS variables, so you can overwrite them or reassign them as you please.

### Color list

<div class="flush grid">
  <div class="column">
    <ul class="color-list">
      <li><span class="swatch" style="background: var(--color-red)"></span> red, <em>danger</em></li>
      <li><span class="swatch" style="background: var(--color-pink)"></span> pink</li>
      <li><span class="swatch" style="background: var(--color-purple)"></span> purple</li>
      <li><span class="swatch" style="background: var(--color-indigo)"></span> indigo, <em>primary</em></li>
      <li><span class="swatch" style="background: var(--color-blue)"></span> blue</li>
      <li><span class="swatch" style="background: var(--color-cyan)"></span> cyan</li>
    </ul>
  </div>
  <div class="column">
    <ul class="color-list">
      <li><span class="swatch" style="background: var(--color-teal)"></span> teal</li>
      <li><span class="swatch" style="background: var(--color-green)"></span> green, <em>success</em></li>
      <li><span class="swatch" style="background: var(--color-lime)"></span> lime</li>
      <li><span class="swatch" style="background: var(--color-yellow)"></span> yellow</li>
      <li><span class="swatch" style="background: var(--color-orange)"></span> orange, <em>warning</em></li>
      <li><span class="swatch" style="background: var(--color-brown)"></span> brown</li>
    </ul>
  </div>
  <div class="column">
    <ul class="color-list">
      <li><span class="swatch" style="background: var(--color-black)"></span> black</li>
      <li><span class="swatch" style="background: var(--color-slate)"></span> slate, <em>text</em></li>
      <li><span class="swatch" style="background: var(--color-grey)"></span> grey, <em>subdued</em></li>
      <li><span class="swatch" style="background: var(--color-light)"></span> light, <em>bg</em></li>
      <li><span class="swatch" style="background: var(--color-white)"></span> white</li>
    </ul>
  </div>
</div>

### Changing colors

You can redefine a color by reassigning its variable in the `:root` selector:

``` css
  :root {
    --color-red: rgb(250,  95,  90);
  }
```

You can remap a state color to a different primary color by reassigning its variable in the `:root` selector:

``` css
  :root {
    --color-primary: var(--color-purple);
  }
```
