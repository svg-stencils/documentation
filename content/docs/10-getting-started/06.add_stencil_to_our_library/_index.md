---
weight: 50
title: Submit a stencil to the SVG Stencil Library
---

## How to add a stencil to the SVG-Stencils library

- Fork the the svg-stencil project ( https://github.com/svg-stencils/svg-stencils.github.io/fork )
- Create your stencil-addition branch (`git checkout -b my-new-stencil`)
- Add your the name and url of your extension to `public/stencils.json`. The files stencil-components.json and stencil-meta.json should exist.

```json
  {
        "name": "My new stencil",
        "url": "https://mipmip.pages.gitlab.gnome.org/my-new-stencil"
  }
```

The the above example implies the existance of these two files:

```
- https://mipmip.pages.gitlab.gnome.org/my-new-stencil/stencil-components.json
- https://mipmip.pages.gitlab.gnome.org/my-new-stencil/stencil-meta.json
```

- Make sure the json is correct, you can test the syntax of the json here: https://jsonlint.com/
- Commit your changes (`git commit -am 'Add new stencil'`)
- Push to the branch (`git push origin my-new-stencil`)
- Create a new Pull Request

**Note**

Only open source stencils are added. We apply a quality check. We preserve the
right to remove stencils from the library at any time. Make sure your are the
author or you are sure the components are allowed to be shared as open source
components.
