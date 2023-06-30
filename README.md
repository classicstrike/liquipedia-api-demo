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

List all pages (10 at a time) by title starting with keyword, in this case `2000`:
https://liquipedia.net/counterstrike/api.php?action=query&list=allpages&apfrom=2000&aplimit=10&format=json

List all pages by category, for example CS1.6 Competitions:
https://liquipedia.net/counterstrike/api.php?action=query&list=categorymembers&cmtitle=Category:CS1.6%20Competitions&format=json

To continue to the next page, update the `cmcontinue` param:
https://liquipedia.net/counterstrike/api.php?action=query&list=categorymembers&cmtitle=Category:CS1.6%20Competitions&format=json&cmcontinue=page|32303031205649525455412043504c204c4154494e20414d4552494341|43466

#### Remember to refer to the latest liquipedia license as they may require you to credit your source etc
