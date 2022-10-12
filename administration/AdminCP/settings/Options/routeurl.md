---
Title: "Site URLs and Routing"
Slug: site-urls-and-routing
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 40
---


## vBulletin URL

This is the URL, or web address, that users will use in their bookmarks or address bar to access your site.<br />
Note: do not add a trailing slash. ('/')




- Variable Name: frontendurl
- Data Type: free
- Default Value: 

## Core URL

The location of your core directory. This directory contains the vBulletin engine and is not public. Do not update unless directed to by vBulletin Support.




- Variable Name: bburl
- Data Type: free
- Default Value: http://www.example.com/forums

## Route Channels and Conversations by Node ID

Use the simplified URL node/xxxx for all channels and conversations (including Forums, Blogs, Social Groups, and Articles). This can be useful if the title values for these node used in the URL cause problems on your site.<br/><br/>

Note that this will override any custom urls configured for Channel or Conversation pages.




- Variable Name: routebynode
- Data Type: free
- Default Value: 0

## Always use Forum URL as Base Path

If this is set to 'Yes' the Forum URL will always be used for links instead of the current URL.  This ensures that links are consistent but may not be desirable if you use multiple domains or a mix of http and https.




- Variable Name: bburl_basepath
- Data Type: boolean
- Default Value: 1

## Redirect Domain Whitelist

Optional, advanced additional URL configuration. This setting should remain blank for most installations. Specify additional domains of your forum:<br />
<br />
Examples:<br />
http://www.example2.com<br />
http://www.example.com<br />
<br />
Note: do not add a trailing slash. ('/')




- Variable Name: redirect_whitelist
- Data Type: free
- Default Value: 

## Disable Redirect Domain Checking

Disable Redirection Checking.  I understand the risks associated with disabling this security feature.




- Variable Name: redirect_whitelist_disable
- Data Type: boolean
- Default Value: 0

## Use ASCII Characters in URLs

This will attempt to transliterate any non-ASCII characters in URLs to ASCII. This includes things like topic titles, channel names, and usernames when used in the URL. For example, this will make changes like <strong>&ntilde;</strong> to <strong>n</strong> and <strong>&egrave;</strong> to <strong>e</strong>.




- Variable Name: asciiurls
- Data Type: boolean
- Default Value: 0

## Redirect 404 pages to root node

Redirect 404 pages to root node




- Variable Name: redirect_404_to_root
- Data Type: free
- Default Value: 0


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>