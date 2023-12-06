# Oracle Support Keyword Bookmarks

## Table of Contents

- [Oracle Support Keyword Bookmarks](#oracle-support-keyword-bookmarks)
  * [Table of Contents](#table-of-contents)
  * [Intro](#intro)
    + [How to setup Keyword Bookmarks](#how-to-setup-keyword-bookmarks)
      - [Chrome](#chrome)
      - [Edge](#edge)
      - [Firefox](#firefox)
  * [Keyword Bookmark URLs](#keyword-bookmark-urls)

## Intro

If you spend a lot of time working on Oracle Support issues, you probably spend a fair amount of that time looking up Oracle Notes, Service Requests, Bugs, Patches and RFCs.

You can use a feature called `keyword bookmarks` in your browser to quickly access those areas of the Oracle Support website, and also any other website such as Service Now, for example.

For example, say you wanted to view DocID 2494259.1 on the Oracle Support website, instead of going to the Oracle Support website, clicking into the search bar, typing the DocID and pressing enter, you could just click into your browser's address bar, press `n` to say you're looking up a note, and then type / paste in the DocID you want to view - you will then be taken directly to the URL for that Note:

![Chrome: Access Keyword Bookmark](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0006a.png)

Press Enter and you will be redirected to the URL for the DocID:

![Chrome: Access Keyword Bookmark](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0006.png)

### How to setup Keyword Bookmarks

#### Chrome

1. Right-click the address bar and choose `Manage search engines and Site Search`:

![Chrome: Manage search engines and Site Search](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0001.png)

2. Scroll down to the `Site Search` heading and click `Add`:

![Chrome: Site Search](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0002.png)

3. Enter new record:
	- Search Engine: Enter name for the Search Engine - e.g. `Oracle Note`
	- Shortcut: `n` (this will be what you enter into the address bar to trigger the keyword bookmark)
	- URL: enter the URL for the bookmark, replacing the part of the URL which would normally contain the content that you'd want to look up with a `%s` (e.g. if the normal URL for a note ishttps://support.oracle.com/rs?type=doc&id=123456.1 then replace `123456.1` with `%s` so the URL will end up as: https://support.oracle.com/rs?type=doc&id=%s
	- Click `Add` to save the record:

![Chrome: Add search engine](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0003.png)

4. The new search engine is listed:

![Chrome: New record added to Site Search list](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0004.png)

5. Add the other records as required ([full list here](#keyword-bookmark-urls)) - they will all end up under the `Site Search` heading:

![Chrome: Updated Site Search list](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0005.png)

#### Edge

The route to add keyword bookmarks to Edge is slightly different.

1. Paste this into the address bar: `edge://settings/searchEngines` and press Enter to access the `Manage search engines` page - then click the `Add` button:

![Edge - Manage search engines](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0007.png)

2. Complete as you would on the steps for Chrome
	- Search Engine: Enter name for the Search Engine - e.g. `Oracle Service Request`
	- Shortcut: `n` (this will be what you enter into the address bar to trigger the keyword bookmark)
	- URL: enter the URL for the bookmark, replacing the part of the URL which would normally contain the content that you'd want to look up with a `%s` (e.g. if the normal URL for a note ishttps://support.oracle.com/rs?type=doc&id=123456.1 then replace `123456.1` with `%s` so the URL will end up as: https://support.oracle.com/rs?type=doc&id=%s
	- Click `Add` to save the record:

![Edge - Manage search engines](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0008.png)

3. Repeat as required for the other keyword bookmarks - [full list here](#keyword-bookmark-urls).

#### Firefox

Follow these instructions to add Keyword Bookmarks in Firefox.

1. Press `CTRL+SHIFT+O` to go to your Bookmarks Library (or go to `Settings > Bookmarks > Manage Bookmarks`)

2. Your Bookmarks library opens. Click into `Other Bookmarks` and then right-click into the right-hand side and choose `Add Folder`:

![Firefox - bookmarks library](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0009.png)

3. Once you're in the `Other Bookmarks` folder, right-click again and click `Add Bookmark`:

![Firefox - bookmarks library](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0010.png)

4. Complete the form:
	- Name: Enter name for the Search Engine - e.g. `Oracle Note`
	- URL: enter the URL for the bookmark, replacing the part of the URL which would normally contain the content that you'd want to look up with a `%s` (e.g. if the normal URL for a note ishttps://support.oracle.com/rs?type=doc&id=123456.1 then replace `123456.1` with `%s` so the URL will end up as: https://support.oracle.com/rs?type=doc&id=%s
	- Keyword: `n` (this will be what you enter into the address bar to trigger the keyword bookmark)
	- Click `Save` to save the record:

![Firefox - Add bookmark](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0011.png)

5. The new bookmark is added - you can edit the values for the bookmark in the lower section of the right-hand side of the screen. Add more records by right-clicking the `Other Bookmarks` folder and choosing `Add Bookmark`.

![Firefox - updated bookmarks library](https://jimpix.co.uk/dist/images/github/keyword-bookmarks/0012.png)

6. Repeat as required for the other keyword bookmarks - [full list here](#keyword-bookmark-urls).

## Keyword Bookmark URLs

```
------------- Saved Searches ---------------

------------- Oracle ---------------

Oracle Bug
b
https://support.oracle.com/rs?type=bug&id=%s

Oracle Note
n
https://support.oracle.com/rs?type=doc&id=%s

Oracle Patch
p
https://support.oracle.com/rs?type=patch&id=%s

Oracle RFC
rfc
https://support.oracle.com/epmos/faces/OnDemandRfcDetail?rfcNumber=%s

Oracle SR
sr
https://support.oracle.com/epmos/faces/SrDetail?srDetailRelativeDateParam=false&srNumber=%s

Oracle Cloud Docs
cloud
https://docs.oracle.com/search/?q=%s&category=cloud&product=en%2Fcloud%2Fsaas%2Ffinancials%2F21d

------------- Service Now ---------------

SNOW Change
ch
https://example.service-now.com/change_request.do?sysparm_query=number=%s

SNOW Incident
in
https://example.service-now.com/incident.do?sysparm_query=number=%s

SNOW Search
srch
https://example.service-now.com/nav_to.do?uri=/$sn_global_search_results.do?sysparm_search=%s


```
