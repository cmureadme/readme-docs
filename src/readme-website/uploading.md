# Uploading

Uploading to the website does not require any programming knowledge or much technical knowledge.
The one thing website unloaders need to understand is markdown formatting.
However, since common platforms like Discord, and Reddit use markdown formatting most people should be familiar with it.
When it doubt Googling how to do format something in markdown is always an option.

As an uploader you will have two responsibilities: creating new author profiles, and digitizing our print content.

## Getting started
The first thing you need to do in order to upload content is get an account on the website.
Ask in the discord and one of the current tech people will be able to make you an account.
From there you go to [cmureadme.com/admin](cmureadme.com/admin) to log into our admin page.

## Creating New Author Profiles
Every single author, both real people and one off bits and jokes they create get uploaded to the website.
It is important to note that whenever we have a new author (ie they write their first article) you need to make their author profile first, before you upload the article that they wrote.
Most of the information fields for an author are not required, this allows you to upload the profile to the website, without needing to wait on the author to give you the information.
However, it is good to get that information from the author, so what I tend to do is upload the new very bare profile and then message the author to get the information.

To add a new author click on the authors button on the left hand side, this will bring you to a table of all of the authors.
Then click the add author button to go to the page to add in a new author.

Here are the data fields and what is required for them:

- Name: This is the author name, this should be pretty self explanatory.
This is a required field.
- Slug: This is the part of the url that takes you to an authors page. 
When a user goes to an authors page it will look like `cmureadme.com/staff/example-author/`.
For the vast majority of authors making their slug in the format `firstname-lastname` works perfectly well, but especially for some of the one off joke characters their names have weirder formatting.
For them just get creative.
This is a required field.
- Img: This is the author profile picture.
If someone hasn't sent you a picture yet, the website will default to showing the `anon.png` image.
This is not a required field.
- Bio: This is the author bio.
It uses markdown formatting, so people can get creative with their bios.
This is not a required field.
- Roles: This defaults to `Staffwriter`, however, if someone primarily makes images you can change it to Staff Artist.
Additionally, sometimes people come up with funny roles, so you can add whatever you want to this.
This is not a required field, but since it has a default it should be filled most of the time.
- Pronouns: This is the pronouns the author uses, this should be pretty self explanatory.
This is not a required field.
- Major: This is the authors major.
This is not a required field.
- Year: This is the authors graduation year.
This is not a required field.
- Location: Authors can send in funny locations.
Authors probably shouldn't dox themselves however.
This is not a required field.
- Fact: A fun fact about the author.
This is not a required field.
- Email: The authors email.
This is not a required field.
- Author status: This is the authors status in the organization.
If this is a real author (ie someones main character they write under) or a heavily reoccurring character they are a `Usual Suspect`.
If this is a one off bit and this character will most likely not reappear and was created for only one article they are an `Independent Contractor`.
Finally if this is a real person who is no longer part of Readme they are an escapee.
This field is required, and it defaults to `Usual Suspect`

When you are done uploading a new author hit the save button on the bottom of the page.
However, if you are uploading multiple authors at once you can hit the save and add another button to save some time.

## Uploading Issues
Issues have a lot of different types of content associated with them.
Because of that it is easiest to upload issues following the order presented below.

Uploading the issue itself:

First go to [the layout repo](https://github.com/cmureadme/readme-layout) and download the most recent issue's full pdf.
It will be named VOLUMEXISSUEYFULL.pdf.
If it is not in the Github repo you can run the `combindme.py` script, instructions found [here](/src/readme-layout/combindme.md).
Or you if you have zero programming experience and are scared ask someone in the Discord to run it.

I recommend having the pdf open in Adobe Acrobat as they make it very easy to copy and paste text from a pdf (this will save you a lot of time later).

Then go back to the admin page and click on the Issues button on the left side, and then click on the add issue button on the right side.

- Name: The name of the issue.
Each issue will be titled `the issue in which blah blah blah` this is the name of the issue.
Upload the this as the name.
It is important to note that you need to upload the full name, which includes the words `the issue in which`.
Make sure to have it in all lowercase, unless the print version specifically has capitalized words.
This field is required.
- Vol: The volume number of this issue.
This field is required.
- Num: The issue number of this issue.
This field is required.
- Archive: This is the pdf of the issue.
Upload the pdf that you downloaded from the Github.
Don't worry what the file is named, as it will be auto named when it is uploaded to our database.
This field is required.
- Release Date: The day that this was published.
This defaults to the current day, so make sure that if you uploading an issue not on the day that it came out that you set it to the correct date.
This field is required.

At the end hit the save button.

Uploading the paid for gag:

The paid for gag is a gag on the first centerfold of the issue.
It goes along the lines `Paid for by: blah blah blah`.
Click on the Paid Fors button on the left side of the screen.
Then click on the add Paid For button on the right side.
There is just one field you need to upload the title.
Just upload the gag, don't include the words `Paid for by:`, its auto included when the website renders.
When you done hit the save button.

Uploading Rejected Headlines:

Click on the rejected headlines button on the left side of the screen.
Then click on the add rejected headline button on the right side of the screen.
This is where it is very handy to have the pdf open in Adobe Acrobat.
You can just copy and paste the rejected headlines into the title field.
The issue field is a drop down menu, select the issue that the rejected headline is associated with.
If you think the rejected headline is particularly funny check the featured box, so it has a high chance to be on the front page.
Since we often have around 10 rejected headlines per issue hitting the save and add another button will save you some time when your uploading them all.

Uploading The Actual Content:

This part is the most time intensive.
It takes 1-2 hours depending on the length of the issue.
I recommend going through the PDF in order page by page, and uploading all of the articles, as that insures you don't forget something.
Also sometimes we will run advertisements for clubs, or for upcoming KGB events.
Because these are time sensitive and also because having ads on the website is something we are in opposition to these ads don't get uploaded to the website.
Also because a lot of editing happens on the actual pdf itself (during the printing process) the articles as they appear in the Google Drive are not the actual fully edited versions.
Because of this you need to copy and paste from the pdf (hence why having Adobe Acrobat is so important).
Another note is that for any of the images that appear in print they will be in [the layout repo](https://github.com/cmureadme/readme-layout) under a folder called images.
However, for the front page cover photo to get the version without text it will most likely be in the Google Drive, or Discord.

A few notes about Adobe Acrobat:

When copy and pasting it often does not properly copy the `-` character, so you will have to manually add that in yourself.
Line breaks will also be messed up when copying and pasting, so you will have to go through and add in the paragraph breaks.

In terms of content we have two types: articles, and image gags.

Uploading Articles:

When you upload articles you want to start on the main page.
Most of our issues will have a magazine style cover.
This cover will have some sort of image along with text along the lines of `Readme Does X`.
When you upload it to the website just upload the cover art without any of the added text.
The article title for that one will be `Readme Does X`.

Here are all of the fields:

- Title: This is the article title.
This is a required field.
- Authors: There can be more than one author per article.
This is not a required field, but the only time that this should be empty is if their is an anonymous author.
- Anon authors: This is the number of anonymous authors for that article.
This is a required field, and is by default set to zero (which is it's most common value).
- Body: This is the actual article text.
It uses markdown formatting.
You should format it to look just like the print layout.
When you want to add an image you put `![](imagename.fileextension)` directly in the text and the image will be loaded there.
This is a required field.
- Slug: This is the part of the url that takes you to an articles page. 
When a user goes to an authors page it will look like `cmureadme.com/article/example-article/`.
The slug should only have a few words in it and often looks like a simplification of the full article title.
This is a required field.
- Issue: This is a drop down menu that lets you choose which issue this was published in.
This is a required field.
- Published: This is a checkbox that lets you uncheck it if an article is not published yet (ie you are uploading it early).
It is by default checked, and in almost all cases you will not need to uncheck it.
- Front page: This is a checkbox that lets you check it if the article you are uploading was on the front page of the print version.
When we do the magazine style of the print version only the cover image is on the front page, but with the newspaper layout there are often one or two articles + an image on the front page.
- Featured: This is a checkbox that lets you check it if you think an article is one of the better articles from that issue.
If you check it will be at the top of the page for that issue + have a higher chance to be featured on the front page of the website.
- Created on: If the article was published on a different date than when the issue was published.
This is not currently used, but would be used if we start uploading online only content.
This is not a required field and for right now don't use it.
- Article images: This allows you to upload image files that are used in the article. 
Before you upload the image files name them something and don't include spaces or other escaped characters.
Whatever you name them is what you need to type into `![](imagename.fileextension)` when you embed them in the body of the article.
This is not a required field.

Uploading Image Gags:

This is for images that stand on their own and have no article attached to them.
They also may have a short caption.

Here are all of the fields:

- Title: This is the article title.
This is a required field.
- Artists: There can be more than one artist per image.
This is not a required field, but the only time that this should be empty is if their is an anonymous artist.
- Anon artists: This is the number of anonymous artists for that image.
This is a required field, and is by default set to zero (which is it's most common value).
- Image: This is where you upload the image file.
This is a required field.
- Alt text: This is where you put the alternative text that describes an image.
This is helpful for people with screen readers and is a nice accessability feature.
This is not a required field.
- Caption: Some images have a short caption others don't.
This uses markdown formatting.
This is not a required field.
- Slug: This is the part of the url that takes you to an images page. 
When a user goes to an authors page it will look like `cmureadme.com/image/example-image/`.
This is a required field.
- Issue: This is a drop down menu that lets you choose which issue this was published in.
This is a required field.
- Published: This is a checkbox that lets you uncheck it if an image is not published yet (ie you are uploading it early).
It is by default checked, and in almost all cases you will not need to uncheck it.
- Front page: This is a checkbox that lets you check it if the image you are uploading was on the front page of the print version.
When we do the magazine style of the print version only the cover image is on the front page, but with the newspaper layout there are often one or two articles + an image on the front page.
- Featured: This is a checkbox that lets you check it if you think an image is one of the better images from that issue.
If you check it will be at the top of the page for that issue + have a higher chance to be featured on the front page of the website.
- Created on: If the article was published on a different date than when the issue was published.
This is not currently used, but would be used if we start uploading online only content.
This is not a required field and for right now don't use it.


This guide is quite long, so if you have any questions always feel free to ask on the Discord.