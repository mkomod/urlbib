
# UrlBib

Takes a given url and returns a formatted bibliography entry. The entry can be piped into a reference file.

## Installation

```
$ git clone https://github.com/mkomod/urlbib
$ export PATH=$PATH:/path/to/urlbib
```

**Note** exporting path does not have a permanent effect. Change your shell rc instead. It is suggested to have a path in your home directory for storing local binaries, in which case just copy over `urlbib`.


## Usage

```
$ urlbib URL REFFERENCE_NAME
```

### example

```
$ urlbib http://www.bibtex.org/Using/ BibTeX:usage

@misc{BibTeX:usage,
	author = {},
	title = {Using BibTeX},
	howpublished = {\url{http://www.bibtex.org/Using/}},
	month = {},
	year = {},
	note = {(Accessed on 07/10/2019)}
}

```

**Note** the output can be piped directly to a bibliography file. 

```
$ urlbib http://www.bibtex.org/Using/ BibTeX:usage >> refs.bib
```


