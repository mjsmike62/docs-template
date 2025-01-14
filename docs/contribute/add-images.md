---
description: Add screenshots and diagrams to the documentation.
sidebar_position: 5
toc_max_heading_level: 3
---

# Add images

You can add [screenshots](#screenshots) and [diagrams](#diagrams) to the ConsenSys documentation.

Add your image to an `assets` or `images` folder within the documentation folder, and link to it in
your doc content using [Markdown syntax](https://docusaurus.io/docs/markdown-features/assets#images).
You can also use HTML to center the image.
For example:

<!--tabs-->

# Markdown

```markdown
<p align="center">

![Snap transaction insights UI](../assets/transaction-insights.png)

</p>
```

# Rendered

<p align="center">

![Snap transaction insights UI](../assets/transaction-insights.png)

</p>

<!--/tabs-->

## Screenshots

Follow the [Rackspace screenshot guidelines](https://docs.rackspace.com/docs/style-guide/screenshots/screenshot-guidelines)
when adding screenshots to the ConsenSys docs.

You might need to re-size your screenshots to make them easy to view and to minimize the file size
for faster page loading:

- Full-width screenshots should be 600-960px wide.
- Vertical, mobile-layout screenshots should be around 360px wide.

## Diagrams

ConsenSys doc sites contain diagrams created using [Figma](https://figma.com/).
You must have access to the ConsenSys **Quorum Diagrams** template files on Figma to create a diagram.

Diagrams can illustrate:

- Detailed or simplified product architecture.
- Technical processes and flows.
- Concept charts and tables.

### Demo

The following video demonstrates creating a diagram for the GoQuorum documentation using Figma:

<p align="center">
  <iframe width="560" height="315" src="https://www.youtube.com/embed/2H-OeBkVOws" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</p>

### Create your Figma diagram

Use the following general guidelines when creating ConsenSys diagrams on Figma.
Refer to the [Figma help website](https://help.figma.com/hc/en-us) for more information on getting started with Figma,
Figma design elements, and more.

#### Basics

- In the **Quorum Diagrams** file on Figma, each page contains diagrams for a different product.
- When creating a new diagram, create a new white frame in the product's page.
  Add frames within the white frame for each iteration of the diagram.
  - For each diagram, create a frame 756px wide using the **Global Background** color (#F6F6F6).
- You can resize a diagram's height, but keep the width at 756px.
  Anchor your elements to the frame using **Left** and **Top** [constraints](https://help.figma.com/hc/en-us/articles/360039957734-Apply-constraints-to-define-how-layers-resize).
- You can [group](https://help.figma.com/hc/en-us/articles/360039832054-Frames-and-Groups) and
  [rename and organize](https://help.figma.com/hc/en-us/articles/360038663994-Name-and-organize-components) elements.

:::tip Tips
- Hold down **Command** on Mac or **Ctrl** on Windows to
  [select](https://help.figma.com/hc/en-us/articles/360040449873-Select-layers-and-objects) elements
  excluding the frame.
- Hold down **Option** and drag to duplicate an element.
:::

#### Design

- Use the pre-made diagram assets as starting points.
  By default, you can adjust the width of the pre-made labels, but the height is automatically sized to the number of
  lines of text.
  To freely customize a component, right-click on it, **detach instance**, and **remove auto layout**.
- Use the pre-defined [color styles](https://help.figma.com/hc/en-us/articles/360039820134-Manage-and-share-styles) or
  black (#00000).
- Use rounded corners of radius 2 for rectangular labels and containers.
- Evenly [align](https://help.figma.com/hc/en-us/articles/360039956914-Adjust-alignment-rotation-and-position) elements.
- Represent similar conceptual elements using similar styles.
  For example, represent two nodes using a dark gradient, and represent two external components using a light gradient.
- You can reuse existing icons from any diagram on any page.
  For example, there are already icons to represent databases, dapps, keys, locks, and logos.

:::tip
Hold down **Shift** when drawing, resizing, and rotating to create perfect horizontal and vertical lines.
:::

#### Text

- Use font **Roboto** for all text.
- Use font sizes between 10–18.
- Use [sentence case](https://docs.microsoft.com/en-us/style-guide/capitalization) in labels and titles.

#### Arrows and lines

- Use a thickness of 2 for arrows, lines, borders, and other strokes.
- Use **Triangle** arrow heads.
- Use straight arrows and lines, with right-angle bends if needed.
  Don't use diagonal arrows and lines.
  If possible, don't overlap arrows and lines.
  To create additional bends in an arrow or line, **detach instance** (if applicable), double-click the arrow or line,
  and click and drag the anchor points.
- Leave about 3px of space between arrow heads and the elements they point to.
  Line ends without arrow heads should touch the connecting element.

:::note example
![Example diagram](../assets/besu-tessera-high-availability.png)
:::

See the
[Figma documentation on the Arrow Tool](https://help.figma.com/hc/en-us/articles/360040450133-Using-Shape-Tools#h_677f8eba-73c4-4987-a64b-c0226aaec392)
for more information.

### Export your Figma diagram

1. Select the frame of your diagram.
   Make sure all elements of your diagram are contained in the frame.
   The name of this frame will be the name of the exported image.
2. Scroll to the bottom of the right sidebar.
   In the **Export** section, choose **2x** scale (for retina screens) and **PNG** or **SVG** file format.
3. Export the diagram to the image folder of the documentation site (for example, `doc.goquorum/docs/assets`).

See [Figma's guide to exports](https://help.figma.com/hc/en-us/articles/360040028114-Guide-to-exports-in-Figma) for more
information.
