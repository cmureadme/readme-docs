# Dependencies
We rely on a few different libraries and packages to run this website.
You can find a current list of them in the `requirments.txt` file.

## Note about `~=`, `>=`, and `==`
- `~=` is used for compatable releases. 
This is generally prefered and should be used unless you have a good reason not to.
- `>=` is used for any version that is the version specified or future relases.
Future relases of a library or package my break things.
Only use this if you have a good reason to
- `==` is used for absolute versions.
Don't use this.
It means you don't get any critical safty updates.
That is bad.

## Django
This is the webframe work we use.
This is a dependacy we will always have.
It is pretty great.

## gunicorn
This is a WSGI server for python.
We use this to run both of our production websites.
We use it along with nginx to host all of the media on the production server.

## Markdown
This allows us to use markdown formating in admin entered text boxes.
We can use markdown formating for example in the body of articles and then when we render it on the html page it is all nice and formated.

## Pillow
This is a python image library.
This is what Django uses to serve images.
We like having images on the website so this is pretty epic.