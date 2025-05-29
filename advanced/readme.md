# 🐙 Advanced Formatting

## Alerts

Alerts are a Markdown extension based on blockquote syntax that you can use to emphasize critical information. They are displayed with distinct colors and icons to indicate the importance of the content.

> [!NOTE]
> Useful information that users should know, even when skimming content.

> [!TIP]
> Helpful advice for doing things better or more easily.

> [!IMPORTANT]
> Key information users need to know to achieve their goal.

> [!WARNING]
> Urgent info that needs immediate user attention to avoid problems.

> [!CAUTION]
> Advises about risks or negative outcomes of certain actions.

## Collapsed Section

You can temporarily collapse sections of your Markdown by creating an expandable section that the reader can choose to expand. For example, when you want to include technical details in an issue comment that may not be relevant or interesting to all readers, you can put those details in a collapsed section.

Any Markdown inside the `<details>` block will be collapsed until the reader clicks to expand the details.

In the `<details>` block, use the `<summary>` tag so readers know what's inside. The label appears to the right of it.

<details>

<summary>Tips for collapsed sections</summary>

### You can add a header

You can add text within a collapsed section.

You can add an image or a code block, too.

```ruby
   puts "Hello World"
```

</details>

## Mermaid Diagrams

Mermaid is a Markdown-inspired tool that turns text into diagrams. For example, Mermaid can interpret flowcharts, sequence diagrams, pie charts, and more.

To create a Mermaid diagram, add the Mermaid syntax inside a fenced code block with the mermaid language identifier.

For example, you can create a flowchart by specifying values and arrows.

Here is a simple flow chart:

```mermaid
graph TD;
    A-->B;
    A-->C;
    B-->D;
    C-->D;
```

## Maps

You can use GeoJSON or TopoJSON syntax to create interactive maps. To create a map, add GeoJSON or TopoJSON in a fenced code block with the geojson or topojson syntax identifier.

```geojson
{
  "type": "FeatureCollection",
  "features": [
    {
      "type": "Feature",
      "id": 1,
      "properties": {
        "ID": 0
      },
      "geometry": {
        "type": "Polygon",
        "coordinates": [
          [
            [
              -90,
              35
            ],
            [
              -90,
              30
            ],
            [
              -85,
              30
            ],
            [
              -85,
              35
            ],
            [
              -90,
              35
            ]
          ]
        ]
      }
    }
  ]
}
```
