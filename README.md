# mdtable2csv (Convert `.md` file to `.csv`)

This is a command-line application written in Python that uses the GitHub markdown API to convert a table in `.md` to `.csv`. The styles also come directly from GitHub, so you'll know exactly how it will appear.

## Motivation

I wanted to convert a table in `.md` to `.csv`, but I can't find any tools on the internet for this purpose. So I thought I can just wrote one.

## Install requirements

```
$ pip install -r requirements.txt
```

**_OR_**

```
$ pip install beautifulsoup4 flask
```

If you have any issues installing Beautiful Soup, visit [this page](http://www.crummy.com/software/BeautifulSoup/bs4/doc/#installing-beautiful-soup).

## Usage

Use the following command to convert `<filename>.md` to `<filename>.csv` :

```
$ ./mdtable2csv <filename>.md
```

And then you will see a `<filename>.csv` in the same folder.

## Examples

### table.md

```markdown
# table.md :
First Header  | Second Header
------------- | -------------
Content Cell  | Content Cell
Content Cell  | Content Cell

$ mdtable2csv table.md

# table.csv :
First Header,Second Header
Content Cell,Content Cell
Content Cell,Content Cell
```

--------------------------------------------------------------------------------

### abc.md

```markdown
# abc.md :
|   |  a | b  | c  |
|---|----|----|----|
| 1 | a1 | b1 | c1 |
| 2 | a2 | b2 | c2 |
| 3 | a3 | b3 | c3 |

$ mdtable2csv abc.md

# abc.csv :
 ,a,b,c
1,a1,b1,c1
2,a2,b2,c2
3,a3,b3,c3
```

--------------------------------------------------------------------------------

**Please give me a star if you find this tool useful, Thank you.**
