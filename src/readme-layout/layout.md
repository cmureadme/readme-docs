# Layout
Readme uses [Scribus](https://sourceforge.net/projects/scribus/) for layout editing, and Github for version control. 

Clone the layout repository:
```
git clone https://github.com/cmureadme/readme-layout.git
```

Readme uses the following fonts, which you should install:

| Font                                                             | Uses                                               |
|------------------------------------------------------------------|----------------------------------------------------|
| [Special Elite](https://fonts.google.com/specimen/Special+Elite) | Titles                                             |
| Courier New                                                      | Centerfold headers, except "the issue in which..." |
| Bell MT                                                          | Everything else                                    |

The layout for the tabloid and each centerfold are done in separate `.sla` files. It's easiest to copy a previous layout as a template.

After adding the new issue's content, use the [Layout checklist](https://docs.google.com/document/d/1e6fiNvDQEVQF29GZjZlifu2QdirIeSB-Vap0Tv_f--c/edit?tab=t.0) to catch common mistakes.

After exporting to PDF, the tabloid needs to be converted to tabloid layout using [this tool](https://momijizukamori.github.io/bookbinder-js/?customSigLength=0&paperSize=TABLOID&sigLength=1&printFile=aggregated&flyleafs=0). Input the 4-page PDF file, don't change any settings, and "Generate PDF Output." 
