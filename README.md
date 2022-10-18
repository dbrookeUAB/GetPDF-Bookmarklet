# GetPDF-Bookmarklet
A bookmarklet function that opens the pdf from the current website of an academic paper

## How
You can either import the `GetPDF` files from this repository or you can make it manually.

Just add a new bookmark and replace the url with the javascript snippet below

```
javascript:void(window.open(document.evaluate("//div/a[contains(@class, \"download\") and starts-with(@href, \"/\") and substring(@href, string-length(@href) - 3)= \".pdf\"]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue,"_blank"))
```

Presto!
