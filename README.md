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


<a href= 'javascript:void(window.open(document.evaluate("//div/a[contains(@class, \"download\") and starts-with(@href, \"/\") and substring(@href, string-length(@href) - 3)= \".pdf\"]",%20document,%20null,%20XPathResult.FIRST_ORDERED_NODE_TYPE,%20null).singleNodeValue.getAttribute(\"href\"),\"_self\"))' >
    <img src="bookmark.svg" width="50" height="50" >
</a>


<a href= 'https://www.google.com' >
    <img src="bookmark.svg" width="50" height="50" >
</a>

