## Grid

Bones comes with a simple grid based on Flexbox. Just put columns in a grid, and they'll expand to fill the available space.

<figure class="small center grid">
  <figcaption>div class="grid"</figcaption>
  {% for i in (1..3) %}
  <div class="padded column" style="background: var(--color-white)">
    div class="column"
  </div>
  {% endfor %}
</figure>

<figure class="small center grid">
  <figcaption>div class="grid"</figcaption>
  {% for i in (1..4) %}
  <div class="padded column" style="background: var(--color-white)">
    div class="column"
  </div>
  {% endfor %}
</figure>

### Sized columns

You can add classes to columns to make them take up a bigger or smaller amount of space.

<figure class="small center grid">
  <figcaption>div class="grid"</figcaption>
  <div class="padded half column" style="background: var(--color-red); color: var(--color-white)">
    class="half column"
  </div>
  {% for i in (1..2) %}
  <div class="padded column" style="background: var(--color-white)">
    class="column"
  </div>
  {% endfor %}
</figure>

<figure class="small center grid">
  <figcaption>div class="grid"</figcaption>
  <div class="padded third column" style="background: var(--color-pink); color: var(--color-white)">
    class="third column"
  </div>
  <div class="padded column" style="background: var(--color-white)">
    class="column"
  </div>
</figure>

<figure class="small center grid">
  <figcaption>div class="grid"</figcaption>
  <div class="padded quarter column" style="background: var(--color-purple); color: var(--color-white)">
    class="quarter column"
  </div>
  <div class="padded column" style="background: var(--color-white)">
    class="column"
  </div>
</figure>

### Flush grids

You can add the `.flush` class to grids to remove the spaces between columns:

<figure class="small center flush grid">
  <figcaption>div class="flush grid"</figcaption>
  {% for i in (1..4) %}
  <div class="padded column" style="background: var(--color-white)">
    div class="column"
  </div>
  {% endfor %}
</figure>
