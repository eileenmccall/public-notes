- The `media` attribute of a `<link>` element tells the browser what media the stylesheet is intended for (e.g. `print`, `tty`)
    - The default is `all`
    - If your stylesheet is not intended for `all` medias, make sure to include the `media` attribute to prevent render-blocking
- Linked or imported stylesheets **must** include a `@charset "UTF-8"` declaration