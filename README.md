# '1.9.4Chem'
Builds on the Original Repo [beloglazov/zotero-scholar-citations](https://github.com/beloglazov/zotero-scholar-citations) and fixed version 1.9.4 by Texot(https://github.com/tete1030). This version removes <sub> and </sub> tags in the titles of papers making it useful for fields like Chemical Engineering and Chemistry which have a lot of compound formulae in title (e.g. H<sub>2</sub>O, CO<sub>2</sub>).

# `00000` Problem in Original Repo [beloglazov/zotero-scholar-citations](https://github.com/beloglazov/zotero-scholar-citations)

The original extension is not working due to new Google robot checking page for some people. In this case, original extension will simply display `00000` for all items instead of notifying this failure. This could be confused with zero citing. A pull request (https://github.com/beloglazov/zotero-scholar-citations/pull/42) was submitted to original repo but has not been merged for months. If you need a fixed version of zotero-scholar-citations, you can download it [here](https://github.com/tete1030/zotero-scholar-citations/raw/my/builds/zotero-scholar-citations-1.9.4-fx.xpi).

This version introduced two changes:

* Fix detection of google robot checking
* Show `No Citation Data` in failure cases instead of `00000`

# Zotero Scholar Citations

This is an add-on for Zotero, a research source management tool. The add-on automatically fetches numbers of citations of your Zotero items from Google Scholar and makes it possible to sort your items by the citations. Moreover, it allows batch updating the citations, as they may change over time.

When updating multiple citations in a batch, it may happen that citation queries are blocked by Google Scholar for multiple automated requests. If a blockage happens, the add-on opens a browser window and directs it to http://scholar.google.com/, where you should see a Captcha displayed by Google Scholar, which you need to enter to get unblocked and then re-try updating the citations. It may happen that Google Scholar displays a message like the following "We're sorry... but your computer or network may be sending automated queries. To protect our users, we can't process your request right now." In that case, the only solution is to wait for a while until Google unblocks you.

Currently, Zotero doesn't have any special field for the number of citations, that's why it is stored in the "Extra" field. To sort by this field you have to add it in the source listing table.

*IMPORTANT:* in version 1.8 the field for storing the number of citations has been changed from "Call Number" to "Extra" -- please update your column configuration.

The add-on supports both versions of Zotero:

1. Zotero Standalone:
  - Download the add-on from https://github.com/tete1030/zotero-scholar-citations/raw/my/builds/zotero-scholar-citations-1.9.4-fx.xpi
  - In Zotero Standalone go to Tools -> Add-ons -> click the settings button in the top-right corner -> Install Add-on From File -> select the downloaded file and restart Zotero.
2. Zotero for Firefox:
  - Install the Firefox add-on from https://addons.mozilla.org/en-us/firefox/addon/zotero-scholar-citations/

Read about how the add-on was made: http://blog.beloglazov.info/2009/10/zotero-citations-from-scholar-en.html

# License

Copyright (C) 2011-2013 Anton Beloglazov

Distributed under the Mozilla Public License (MPL).
