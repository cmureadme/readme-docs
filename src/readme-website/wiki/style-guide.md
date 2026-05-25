# Style Guide

- Use 4-space indents everywhere.
- Please comment things that need extra explanation.
- Write Python functions and variables in `snake_case`, not `camelCase`. Classes are still in `PascalCase`.
- Anything in HTML/CSS (including django variables e.g. `{% block head-content %}`) should be in `kebab-case`
- HTML styling should be in separate files from the HTML.
  - A file named `.../foo.html` should should place its corresponding styling in `static/styles/foo.css`
- MAKE AT LEAST SOME effort to write efficient/clean code. People will work with it later. These people might be you.
