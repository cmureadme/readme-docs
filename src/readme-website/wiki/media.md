# Media
Media for the readme website is stored in one of two places: `static/` or `media/`. `media/` is not stored in the [`readme-website`](https://github.com/cmureadme/readme-website) repo.

`static/` contains  images necessary for the website to function.

`media/` contains everything uploaded through the Django interface.

- `author_images`
These are the profile pictures for all of the authors.
When you upload an author profile picture `foo.png` it is stored in `media/author_images/foo.png`.

- Magazine PDFs
The PDFs of the print version of the magazine are renamed on upload.
They are stored as `media/volX/issueY/CMURREADME_VOLX_ISSUEY.pdf`.

- Article Images
Article images are not renamed on upload.
When you reference an image `bar.png` in an article you do so by including `{{bar.png}}` in the article body where you want the image to appear.
An image published in vol X issue Y is stored in `media/volX/issueY/images/`.