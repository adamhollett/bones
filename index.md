---
---

{% include readme.md %}

---

## Typography spacing

Bones uses a typography grid inspired by Richard Rutter's article [Compose to a Vertical Rhythym](https://24ways.org/2006/compose-to-a-vertical-rhythm). The basic principle is that text sizes and spaces should be a multiple of some base value. Larger textual elements have larger spaces around them.

Spacing CSS variables:
- `--base-font-size` <span id="base-font-size-value"></span>
- `--base-line-height` <span id="base-line-height-value"></span>

The basic space unit is equal to `--base-font-size` * `--base-line-height`. By default this is 32px.

## Typography scaling

Text and heading sizes grow on a gradual scale. Each level of heading, ascending from h4 to h1, is larger than the previous by a factor of `--scale-factor`.

Scaling CSS variables:
- `--scale-factor` <span id="scale-factor-value"></span>

### Scale examples

> #### Heading 4
>
> Fourth-level headings are the same size as body text and have no line space between them and the content that follows.

> ### Heading 3
>
> Third-level headings are larger than body text and have no line space between them and the content that follows.

> ## Heading 2
>
> Second-level headings are larger than third-level and have one line space between them and the content that follows.

> # Heading 1
>
> The top-level heading is the largest and has two line spaces between it and the content that follows.

## Font stacks

The font stacks in Bones come from Ire Aderinokun's article [The New System Font Stack?](https://bitsofco.de/the-new-system-font-stack/) and include reasonable stacks of system fonts in sans serif, serif, and monospace.

Font CSS variables:
- `--fonts-sans` <span id="fonts-sans-value"></span>
- `--fonts-serif` <span id="fonts-serif-value"></span>
- `--fonts-mono` <span id="fonts-mono-value"></span>

## Responsive images and videos

Images and videos won't exceed their container width by default.

![](https://picsum.photos/1200/400/?blur)

<script>
  const rootStyles = getComputedStyle(document.documentElement);

  const baseFontSize = rootStyles.getPropertyValue("--base-font-size").trim();
  document.getElementById("base-font-size-value").innerText = `(${baseFontSize})`;

  const baseLineHeight = rootStyles.getPropertyValue("--base-line-height").trim();
  document.getElementById("base-line-height-value").innerText = `(${baseLineHeight})`;

  const scaleFactor = rootStyles.getPropertyValue("--scale-factor").trim();
  document.getElementById("scale-factor-value").innerText = `(${scaleFactor})`;

  const fontsSans = rootStyles.getPropertyValue("--fonts-sans").trim();
  document.getElementById("fonts-sans-value").innerText = `(${fontsSans})`

  const fontsSerif = rootStyles.getPropertyValue("--fonts-serif").trim();
  document.getElementById("fonts-serif-value").innerText = `(${fontsSerif})`

  const fontsMono = rootStyles.getPropertyValue("--fonts-mono").trim();
  document.getElementById("fonts-mono-value").innerText = `(${fontsMono})`
</script>
