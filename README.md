# 🧩 Layer Structure Exporter (Configurable)

>This Plugin was created with the help of chatgpt.

A Figma plugin that extracts the hierarchical **structure of all layers, groups, and components** from your current page — with **optional metadata** like bounding boxes, colors, opacity, fonts, and more.

---

## ✨ Features

- 📂 View and export a full **layer tree** (frames, groups, nested layers, etc.)
- 🧠 Optionally include metadata:
  - Bounding box (x, y, width, height)
  - Fill colors
  - Strokes
  - Opacity
  - Corner radius
  - Font name and size
  - Visibility
  - Node IDs
  - Text content
- 💾 **Download as JSON** with only the fields you select.
- ⚙️ Works on the free Figma plan.

---

## Screenshot
![Figma Layer Structure Explorer](./screenshots/Figma%20Layer%20structure%20explorer%20.png "Optional Title")


## 🖼️ Example Output

```json
{
  "name": "Login Page",
  "type": "PAGE",
  "children": [
    {
      "name": "Header",
      "type": "FRAME",
      "bounds": { "x": 0, "y": 0, "width": 1440, "height": 80 },
      "fills": [{ "type": "SOLID", "color": { "r": 1, "g": 1, "b": 1 } }],
      "children": [
        {
          "name": "Title",
          "type": "TEXT",
          "text": "Welcome Back",
          "fontName": { "family": "Inter", "style": "Bold" },
          "fontSize": 24
        }
      ]
    }
  ]
}
