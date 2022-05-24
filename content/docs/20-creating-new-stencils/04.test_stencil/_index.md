---
weight: 40
title: Test your Stencil
---

## Test your stencil

If you can run a (local) webserver you can test your stencil in the SVG
Stencils Web App. Your stencil URL is the url pointing to the parent directory
of stencil-meta.json and stencil-components.json. Add this URL as query
parameter to the svg-stencils-url.

```
# Mac
open https://svg-stencils.github.io/?stencil=http://localhost:8080

# Linux
xdg-open https://svg-stencils.github.io?stencil=http://localhost:8080
```

Not all local webservers work. `http.server` with cors enabled has been proven to work from a
local address.

```
cd my-stencil-directory
npm exec http-server -- --cors
```

