# Settings
Django supports having multiple different settings files for different contexts.
All of the settings files are python files placed in `settings/`.
In general, you should not need to edit any of the settings files.

---

## Base
`base.py` contains the base settings that apply to every instance of the website.
The bulk of our settings live in this file, because there are not many settings that are dependent on the hosting context.

## Host
`host.py` contains the settings that are needed when running on a server, and not your local machine.
It extends `base.py`.

### Production
`prod.py` contains the settings that are needed for running on our main production website.
It extends `host.py`.

### Staging
`staging.py` contains the settings that are needed for running our staging website.
It extends `host.py`.

## Local
`local.py` contains the settings that are needed for running the website on your local machine.
It extends `base.py`.