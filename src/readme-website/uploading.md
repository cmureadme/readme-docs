# Uploading
Uploading to the website uses Markdown. 
This does not require any programming knowledge or much technical knowledge.

As an uploader you are responsible for creating new author profiles and digitizing our print content.
## Getting started
Ask in the discord to have one of the current tech people make you an account.
Then, go to [cmureadme.com/admin](cmureadme.com/admin) to log into our admin page.
## Creating New Author Profiles
Every single author gets uploaded to the website. This includes both recurring authors and one-off joke characters.

The article's author profile must exist before the article is uploaded. Create a mostly blank profile before uploading articles, then message the author for the rest of the information (which can be filled in afterwards). 

To add a new author, click on the "authors" button on the left hand side.
Then, click the "add author" button.

##### Author data fields
| Field          | Description                                                                                                                           |
|----------------|---------------------------------------------------------------------------------------------------------------------------------------|
| Name*          | The author's name                                                                                                                     |
| Slug*          | The part of the url that takes you to an authors page. For example, `firstname-lastname` in `cmureadme.com/staff/firstname-lastname/` |
| Img            | The author's profile picture. Defaults to [anon.png](https://cmureadme.com/media/author_images/anon.png)                              |
| Bio            | The author's bio                                                                                                                      |
| Roles          | Any roles the author has. Defaults to `Staffwriter`                                                                                   |
| Pronouns       | The author's pronouns                                                                                                                 |
| Major          | The author's major                                                                                                                    |
| Year           | The author's graduation year                                                                                                          |
| Fact           | A fun fact about the author                                                                                                           |
| Email          | The author's email                                                                                                                    |
| Author status* | The author's status in the organization. Defaults to `Usual Suspect`                                                                  |

_*required_

For Author status, if the author is a real person or frequently reoccurring character they are a `Usual Suspect`.
If they are a one-off bit, they are an `Independent Contractor`.
Finally, if this is a real person who is no longer part of Readme they are an `Escapee`.

When you are done entering information, hit the "save" button on the bottom of the page. 
If you are uploading multiple authors sequentially, you can hit the "save and add another" button.

## Uploading Issues of Readme
First, go to [the layout repo](https://github.com/cmureadme/readme-layout) and download the most recent issue's full pdf.
It will be named `VOLUME#ISSUE#FULL.pdf`.

If it is not in the Github repo, you can run the [`combineme.py`](/src/readme-docs/readme-layout/combineme.html) script.
If you need help, ask someone in the Discord to run it.

I recommend having the pdf open in Adobe Acrobat as it makes it very easy to copy and paste text from the pdf.

Click on the "Issues" button on the left side of the admin page, then click on the "add issue" button on the right side.

##### Issue data fields
| Field         | Description                                                                                                                                |
|---------------|--------------------------------------------------------------------------------------------------------------------------------------------|
| Name*         | The title of the issue, starting with `the issue in which`. Ex. `the issue in which we promise you that our alibi holds up under scrutiny` |
| Vol*          | The volume number                                                                                                                          |
| Num*          | The issue number                                                                                                                           |
| Archive*      | The complete pdf of the issue                                                                                                              |
| Release Date* | The publication date of the issue. Defaults to the current day, so make sure to double-check                                               |

Make sure to hit the save button.

### "Paid for" gag:
The "paid for" gag is a gag on the first centerfold of the issue. Ex. `Paid for by: Extensive lawyer fees and two bungled investigations`

Click on the Paid Fors button on the left side of the screen.
Then, click on the add Paid For button on the right side and enter the gag. Don't include the words `Paid for by:`.

Make sure to hit save.

### Rejected Headlines
Click on the rejected headlines button on the left side of the screen.
Then, click on the add rejected headline button on the right side of the screen.
Copy and paste the rejected headlines into the title field.
Select the issue that the rejected headline is associated with.
If you think the rejected headline is particularly funny, check the featured box, so it has a high chance to be featured on the homepage.
Make sure to save.

### Uploading Articles and Images:
This part is the most time intensive, taking 1-2 hours depending on the length of the issue.
Going through the PDF in order page by page ensures that you don't forget something.


#### Uploading Articles:
When you upload articles you want to start on the main page.

Because copy editing happens on the actual pdf itself, the articles as they appear in the Google Drive are not the final versions, so copy text from the pdf.

The hyphen character (`-`) is often not copied properly, so you have to manually add that in.
Line breaks will also be messed up, so you have to go through and add in the paragraph breaks.
##### Article data fields
| Field          | Description                                                                                                                               |
|----------------|-------------------------------------------------------------------------------------------------------------------------------------------|
| Title*         | The title of the article                                                                                                                  |
| Authors        | The article's authors. Leave empty if the author is anonymous.                                                                            |
| Body*          | The article text in markdown format.                                                                                                      |
| Slug*          | The part of the url that takes you to an article's page. Ex. `example-article` in `cmureadme.com/article/example-article/`                |
| Issue*         | The issue the article was published in                                                                                                    |
| Published      | Whether the article is published. True by default. Uncheck only if the article is uploaded prior to publication.                          |
| Front page     | Whether the article was on the front page. For "magazine" layouts, only the cover image is on the front page.                             |
| Featured       | Whether the article is featured. This puts it at the top of its issue's page and increases the chances of being featured on the homepage. |
| Created on     | Unused. The date the article was published, if different from the issue.                                                                  |
| Article images | Any images associated with the article                                                                                                       |

_*required_

Any images associated with the article should be embedded with `![](filename.ext)`. For example, `![](anon.png)` embeds `anon.png`. The files can be found in [the layout repo](https://github.com/cmureadme/readme-layout) in the issue folder in a folder called `images`.

#### Uploading Images:
This is for images that stand on their own and have no article attached to them. They also may have a short caption.

Front cover art should be uploaded without any of the added text. The version without text will most likely be in the Google Drive. If it's not, contact the artist to upload it to the Drive.

The files can be found in [the layout repo](https://github.com/cmureadme/readme-layout) in the issue folder in a folder called `images`.
However, for the front cover, 

Sometimes, we run advertisements for upcoming KGB events or for other clubs. 
These don't get uploaded to the website.

##### Image data fields

| Field              | Description                                                                                                                             |
|--------------------|-----------------------------------------------------------------------------------------------------------------------------------------|
| Title*             | The title of the image                                                                                                                  |
| Artists            | The image's artists. Leave empty if the author is anonymous.                                                                            |
| Anonymous artists* | The number of anonymous artists. Defaults to 0                                                                                          |
| Image*             | The image file                                                                                                                          |
| Alt text           | Accessible text describing the image for screenreaders.                                                                                 |
| Caption            | The image caption in markdown format                                                                                                    |
| Slug               | The part of the url that takes you to an image's page. Ex.  `example-image`  in  `cmureadme.com/image/example-image/                    |
| Issue              | The issue the image was published in                                                                                                    |
| Published          | Whether the image is published. True by default. Uncheck only if the image is uploaded prior to publication.                            |
| Front page         | Whether the image was on the front page. For "magazine" layouts, only the cover image is on the front page.                             |
| Featured           | Whether the image is featured. This puts it at the top of its issue's page and increases the chances of being featured on the homepage. |
| Created on         | Unused. The date the image was published, if different from the issue.   

_*required_

If you have any questions, ask them in the [Discord](cmukgb.org/readme).
