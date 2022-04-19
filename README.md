
# scrape.sh

Wrapper for https://github.com/lawzava/scrape to scrape a TSV (tab seperated file) of 
urls to product a TSV output with emails

### Ideal scrape.sh usage

./scrape.sh{php} -f 2 file.tsv 
options
-f email column number (defaults = 1)
-v will output to stderr debug information

ouptput to stdout:
```
email     domain    website
```



## Forked from https://github.com/lawzava/scrape

CLI utility to scrape emails from websites

### Usage
Sample call:

`scrape -w https://lawzava.com` 

Depends on `chromium` or `google-chrome` being available in path if `--js` is used

#### Parameters:
```
          --async             Scrape website pages asynchronously (default true)
      -d, --depth int         Max depth to follow when scraping recursively (default 3)
          --emails            Scrape emails (default true)
          --follow-external   Follow external 3rd party links within website
      -h, --help              help for scrape
          --js                Enables JS execution await
          --debug             Print debug logs
          --recursively       Scrape website recursively (default true)
      -w, --website string    Website to scrape (default "https://lawzava.com")
```
