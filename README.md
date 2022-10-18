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

[Hello Bookmarklet]("javascript:void\(window.open\(document.evaluate\('//div/a\[contains\(@class,\'download\'\) and starts-with\(@href, \'/\'\) and substring\(@href, string-length(@href\) - 3)= \'.pdf\'\]',document,null,XPathResult.FIRST_ORDERED_NODE_TYPE,null\).singleNodeValue,'_blank'\)\) ;")
