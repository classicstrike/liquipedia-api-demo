# liquipedia-api-demo
Useful demo endpoints to help get started with the liquipedia API

Ref: https://liquipedia.net/counterstrike/api.php?action=help&modules=parse

Get the full page:
https://liquipedia.net/counterstrike/api.php?action=parse&page=2001_CPL_Europe_London&format=json

Get the sections on a page:
https://liquipedia.net/counterstrike/api.php?action=parse&page=2001_CPL_Europe_London&prop=sections&format=json

Get a specific section on a page:
https://liquipedia.net/counterstrike/api.php?action=parse&page=2001_CPL_Europe_London&prop=sections&section=4&format=json

Get the links from a specific section on a page:
https://liquipedia.net/counterstrike/api.php?action=parse&page=2001_CPL_Europe_London&prop=links&section=4&format=json

Get the section in XML format:
https://liquipedia.net/counterstrike/api.php?action=parse&page=2001_CPL_Europe_London&prop=parsetree&section=4&format=json

To list all the tournaments or players in particular, you have to find a page that lists them and remember to use the `continue` param:
https://liquipedia.net/counterstrike/api.php?action=parse&page=2001_CPL_Europe_London&format=json&continue=
