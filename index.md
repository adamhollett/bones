---
---

{% include readme.md %}

---

## Typography spacing

Bones uses sensible, legible sizes for text by default. The base font size is 1.25rem, which translates to 20px if unchanged. The base line-height is 1.5, which results in a line height of 30px.

The default space unit, just called `--space`, defaults to the font size multiplied by the line height: 30px.

Spacing CSS variables:
- `--base-font-size` <span id="base-font-size-value"></span>
- `--base-line-height` <span id="base-line-height-value"></span>
- `--space` <span id="space-value"></span>

## Typography scaling

Text and heading sizes grow on a gradual scale. Each level of heading, ascending from h4 to h1, is larger than the previous by a factor of `--scale-factor`. Larger headings have larger margins.

Scaling CSS variables:
- `--scale-factor` <span id="scale-factor-value"></span>

### Scale examples

> #### Heading 4
>
> Fourth-level headings are the same size as body text.

> ### Heading 3
>
> Third-level headings are larger than body text and have top and bottom margins.

> ## Heading 2
>
> Second-level headings are larger than third-level and have top and bottom margins.

> # Heading 1
>
> The top-level heading is the largest and has the largest margins.

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

  const space = rootStyles.getPropertyValue("--space").trim();
  document.getElementById("space-value").innerText = `(${space})`;

  const scaleFactor = rootStyles.getPropertyValue("--scale-factor").trim();
  document.getElementById("scale-factor-value").innerText = `(${scaleFactor})`;

  const fontsSans = rootStyles.getPropertyValue("--fonts-sans").trim();
  document.getElementById("fonts-sans-value").innerText = `(${fontsSans})`

  const fontsSerif = rootStyles.getPropertyValue("--fonts-serif").trim();
  document.getElementById("fonts-serif-value").innerText = `(${fontsSerif})`

  const fontsMono = rootStyles.getPropertyValue("--fonts-mono").trim();
  document.getElementById("fonts-mono-value").innerText = `(${fontsMono})`
</script>
