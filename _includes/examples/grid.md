## Grid

Bones comes with a simple grid based on Flexbox. Just put columns in a grid, and they'll expand to fill the available space.

<div class="small center grid">
  {% for i in (1..3) %}
  <div class="padded column" style="background: var(--color-bg)">
    div class="column"
  </div>
  {% endfor %}
</div>

<div class="small center grid">
  {% for i in (1..4) %}
  <div class="padded column" style="background: var(--color-bg)">
    div class="column"
  </div>
  {% endfor %}
</div>

You can add classes to columns to make them take up a bigger or smaller amount of space.

`.half.column`

<div class="small center grid">
  <div class="padded half column" style="background: var(--color-red)">
    class="half column"
  </div>
  {% for i in (1..2) %}
  <div class="padded column" style="background: var(--color-bg)">
    class="column"
  </div>
  {% endfor %}
</div>

`.third.column`

<div class="small center grid">
  <div class="padded third column" style="background: var(--color-pink)">
    class="third column"
  </div>
  {% for i in (1..3) %}
  <div class="padded column" style="background: var(--color-bg)">
    class="column"
  </div>
  {% endfor %}
</div>

`.quarter.column`

<div class="small center grid">
  <div class="padded quarter column" style="background: var(--color-purple)">
    class="quarter column"
  </div>
  {% for i in (1..2) %}
  <div class="padded column" style="background: var(--color-bg)">
    class="column"
  </div>
  {% endfor %}
</div>
