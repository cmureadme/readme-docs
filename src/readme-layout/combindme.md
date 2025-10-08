# combindme

combindme is a very simple python script to properly combind each of the individual pdfs meant for printing into one pdf to put on the website.

## Getting combindme to work
This section assumes you have never used python or a command line before (but that's ok).

combindme is a python script which means you need to have python installed on your computer.
Go to the [offical page](https://www.python.org/downloads/) to download the newest version of python.

Now that you have python installed we need to install 2 packages.

If you are on Windows open the terminal and run:
```
pip install argparse
pip install pypdf
```

If you are on Linux or Mac open the terminal and run:
```
pip3 install argparse
pip3 install pypdf
```

## Using combindme
combindme expects pdf files to be formated in a certain way.
The tabloid file should be 4 pages.
It is passed in with the `-t` flag.
The first two pages will be the first two pages of the outputed pdf file.
The last two pages will be the last two pages of the outputed pdf file.

combindme takes two optional pdf arguments.
These are for the centerfolds.
It expects the centerfolds to each be two pages.
Centerfold one will be placed before centerfold 2 in the outputed pdf file.
Centerfold one is passed in with the `-c1` flag and centerfold two is passed in with the `c2` flag.

There are 3 other required arguments.
You need to pass in the volume number with the `-v` flag.
You need to pass in the issue number with the `-i` flag.
You also need to pass in the destination path of where the outputed pdf file will go in the `-d` flag.

The outputed pdf will be named `VOLUMEvISSUEiFULL.pdf` where `v` and `i` are the numbers passed into the `-v` and `-i` flags.

If you ever forget any of this information you can run the script with the `-h` flag.

On Windows this looks like:
```
python combindme.py -h
```

On Linux or Mac this looks like:
```
python3 combindme.py -h
```

Here is a sample running of combindme on Windows:
```
python3 combindme.py -v 1 -i 1 -t path\to\tabloid.pdf -c1 path\to\centerfold1.pdf -c2 path\to\centerfold2.pdf -d path\to\destination\folder\
```

Here is a sample running of combindme on Linux or Mac:
```
python3 combindme.py -v 1 -i 1 -t path/to/tabloid.pdf -c1 path/to/centerfold1.pdf -c2 path/to/centerfold2.pdf -d path/to/destination/folder/
```

NOTE: If you have never used the command line before it might seem annoying to type out long paths by hand.
Once you have enough of the path typed out you can use the tab key to autocomplete the rest of the path.