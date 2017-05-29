## Typography

Bones keeps things simple and gives headings plenty of space to breathe by using a [modular grid](https://www.gridlover.net). Bones defines styles for heading levels 1–4. If you need styles for levels 5 and 6, you can write your own.

{% for i in (1..4) %}
  <figure>
    <h{{ i }}>Heading {{ i }}</h{{ i }}>
    <p>The quick brown fox jumps over a lazy dog.</p>

    <figcaption>Heading level {{ i }}</figcaption>
  </figure>
{% endfor %}
