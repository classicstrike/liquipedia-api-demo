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

If someone figures out how to use the API to get more specific information such as tournaments, players, etc please share!
