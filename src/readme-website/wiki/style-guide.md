# Style Guide

- 4 space indents everywhere
- please comment things that need extra explanation
- write python functions and variables in `snake_case`, not `camelCase`. Classes are still in `PascalCase`.
- anything in HTML/CSS (including django variables e.g. `{% block head-content %}`) should be in `kebab-case`
- HTML styling for should be in separate files from the HTML.
  - a file named `.../foo.html` should should place its correspondidng styling in `static/styles/foo.css`
