# Media
Media for the readme website is stored in one of two places: `static/` or `media/`.

## `static/`
This contains only a few images.
These are not user uploaded content but rather images the website needs to display.
This includes images for the favicon, and some logo images for a few of the pages.

## `media/`
This is where the vast majority of all of the media we have is stored.
All of the media in here is user uploaded through the Django Admin interface.

### `author_images`
These are the profile pictures for all of the authors.
When you upload an author profile picture `foo.png` it is stored in `media/author_images/foo.png`.

### Magazine PDFs
The pdfs of the print version of the magazine are renamed on upload, so it does not matter what you call them.
For vol X issue Y the pdf is named `CMURREADME_VOLX_ISSUEY.pdf`.
It is stored in `media/volX/issueY/CMURREADME_VOLX_ISSUEY.pdf`.

### Article Images
Article images are not renamed on upload it does matter what you call them, don't name them something stupid.
When you refrance an image `bar.png` in an article you do by writting {{bar.png}} in the article body where you want the image to appear.
For the image `bar.png` that was published in vol X issue Y it is stored in `media/volX/issueY/images/bar.png`.