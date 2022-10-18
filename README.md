# GetPDF-Bookmarklet
A bookmarklet function that opens the pdf from the current website of an academic paper

## How
You can either import the `GetPDF` files from this repository or you can make it manually.

Just add a new bookmark and replace the url with the javascript snippet below

```
javascript:(function(){if(document.evaluate("//a[starts-with(@href,%20'/action/showPdf')]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue%20!=%20null){window.open(document.evaluate("//a[starts-with(@href,%20'/action/showPdf')]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue.getAttribute('href'),'_self');}else%20if(%20document.evaluate("//a[((starts-with(@href,%20\"/\")%20and%20substring(@href,%20string-length(@href)%20-%203)=%20\".pdf\")%20and%20not(contains(@href,\"suppl\")))%20or%20(contains(@class,\"download\")%20and%20contains(@href,\"pdf\"))%20or%20(contains(@href,\"/pdf\")%20and%20contains(@href,\"?download=true\"))%20or%20starts-with(@href,\"/doi/pdf/\")]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue%20!=%20null){window.open(document.evaluate("//a[((starts-with(@href,%20\"/\")%20and%20substring(@href,%20string-length(@href)%20-%203)=%20\".pdf\")%20and%20not(contains(@href,\"suppl\")))%20or%20(contains(@class,\"download\")%20and%20contains(@href,\"pdf\"))%20or%20(contains(@href,\"/pdf\")%20and%20contains(@href,\"?download=true\"))%20or%20starts-with(@href,\"/doi/pdf/\")]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue.getAttribute('href').replace('download=true','download=false'),'_self');}else%20if(document.evaluate("//a[(contains(@href,%20\"com.ezproxy3.\")%20and%20(substring(@href,%20string-length(@href)%20-%203)=%20\".pdf\")%20or%20(contains(@href,\"/pdf\")%20and%20contains(@href,%20\"?download=true\")))]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue%20!=%20null){window.open(document.evaluate("//a[(contains(@href,%20\"com.ezproxy3.\")%20and%20(substring(@href,%20string-length(@href)%20-%203)=%20\".pdf\")%20or%20(contains(@href,\"/pdf\")%20and%20contains(@href,%20\"?download=true\")))]",document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null).singleNodeValue.getAttribute("href").replace("download=true","download=false"),'_self')}})();
```

Presto!
