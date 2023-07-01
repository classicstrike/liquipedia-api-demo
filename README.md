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

You can also visit the [Search by property](https://liquipedia.net/counterstrike/Special:SearchByProperty) page to build quieries like this which are more efficient and less prone to API Rate Limiting:

#### List teams in tournament
https://liquipedia.net/counterstrike/api.php?action=askargs&format=json&conditions=Is%20result%20type%3A%3Ateam%7C-Has%20subobject%3A%3A2001_CPL_Europe_London&printouts=Has%20team%20page

#### List all CS 1.6 teams (offet 0-50 limit)
https://liquipedia.net/counterstrike/api.php?action=askargs&format=json&parameters=offset%3D0|limit%3D50&conditions=Has%20cs::true&printouts=Has%20team%20name|Has%20location|Was%20created|Was%20disbanded

#### Remember to refer to the latest liquipedia license as they may require you to credit your source etc
