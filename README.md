# GetPDF-Bookmarklet
A bookmarklet function that opens the pdf from the current website of an academic paper

## How
You can either import the `GetPDF` files from this repository or you can make it manually.

This is a regular paragraph.

<table>
    <tr>
        <td>Foo</td>
    </tr>
</table>

This is another regular paragraph.


<a href="javascript:void(window.open(document.evaluate('//div/a[not(contains(@href,%20"epdf"))%20and%20contains(@href,%20"pdf")%20and%20starts-with(@href,%20"/")]',%20document,%20null,%20XPathResult.FIRST_ORDERED_NODE_TYPE,%20null).singleNodeValue.getAttribute('href'),'_self'))""><img src="bookmark.svg" width="50" height="50" ></a>

