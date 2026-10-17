# Eze-IO Resources

A responsive static webpage that lists files, designs and media as searchable cards.

**[Open the webpage →](https://eze-io.github.io)**

## Features

- Responsive card grid that works on phones, tablets and desktops
- Live search by resource name or URL
- Light and dark mode (follows your system setting, with a toggle)
- Image previews and file-type icons

## Adding a resource

Resources are loaded from [`misc/resources.json`](misc/resources.json). Add a `"Name": "URL"` pair to the `items` object:

```json
{
  "title": "resources",
  "items": [{
    "Eze-IO Logo": "https://eze-io.github.io/misc/package/logo.svg",
    "My New File": "https://eze-io.github.io/path/to/file.pdf"
  }]
}
```

## Running locally

The page fetches the JSON file, so serve it over HTTP instead of opening `index.html` directly:

```bash
python3 -m http.server 8000
```

Then visit http://localhost:8000.

## Built with

- [Tailwind CSS](https://tailwindcss.com)
- [Font Awesome](https://fontawesome.com)
