# combineme

combineme is a very simple python script to properly combine each of the individual PDFs meant for printing into one pdf to put on the website.

In `readme-layout`, run
```
pip install -r requirements.txt
```

To combine PDFs, run with the desired volume, issue, pdf paths, and destination
```
python3 combineme.py -v [#] -i [#] -t path/to/tabloid.pdf -c1 path/to/centerfold1.pdf -c2 path/to/centerfold2.pdf -d path/to/destination
```
The outputted pdf will be named `VOLUME[v]ISSUE[i]FULL.pdf`.

To review the flags, run
```
python combineme.py -h
```

## combineme.py flags
\**required*

| Flag                  | Description                           |
|-----------------------|---------------------------------------|
| *`-v`,`--volume`      | Volume number                         |
| *`-i`,`--issue`       | Issue number                          |
| *`-d`,`--destination` | Destination location for combined pdf |
| *`-t`,`--tabloid`     | Path to existing 4-page tabloid pdf   |
| `c1`,`--centerfold1`  | Path to first 2-page centerfold pdf   |
| `c2`,`--centerfold2`  | Path to second 2-page centerfold pdf  |
| `c3`,`--centerfold3`  | Path to third 2-page centerfold pdf   |
