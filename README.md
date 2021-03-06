# ePublius
Generates a stylised HTML site from an ePub book

## Usage

```bash
./epublius.py -p prefix -s suffix -f 02_title.html -t 06_toc.html -b https://www.openbookpublishers.com/product/97 -d ../epub/OEBPS/ -o ../epub/new/ -h header_add
```

Alternatively, one can use `epublius_wrapper.py` to discover the values of parameters to be given to `epublius.py`:

```bash
./epublius_wrapper.py -p prefix -s suffix -h header_add -b https://www.openbookpublishers.com/product/97 -f 9781906924737_Oral_Literature_in_Africa.epub -o test
```


### Parameters


| Parameter | Description                                                               |
|-----------|---------------------------------------------------------------------------|
| `-p`      | File containing prefix                                                    |
| `-s`      | File containing suffix                                                    |
| `-b`      | URL of book's page                                                        |
| `-t`      | TOC file                                                                  |
| `-f`      | Frontpage file                                                            |
| `-d`      | Directory prefix (of content, not prefix/suffix)                          |
| `-o`      | Target directory                                                          |
| `-h`      | File containing HTML to inject into header                                |
| `-n`      | Title name                                                                |
| `-c`      | A colophon file (e.g., the license). There may be  multiple -c parameters |
| `-r`      | How much to resize the images (as percentage; default is 50).             |
| `-i`      | Index file to use                                                         |
| `-u`      | URL path of this book                                                     |
| `-k`      | Copyright file                                                            |
| `-a`      | Donation link                                                             |

