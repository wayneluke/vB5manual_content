---
Title: "Style and Language Settings"
Slug: style-language-settings
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 130
---


## Default Language

Select the default language for your forums. This language will be used for all guests, and any members who have not expressed a language preference in their options.




- Variable Name: languageid
- Data Type: number
- Default Value: 1

## Default Style

Select the default style for your forums. This style will be used for all guests, and any members who have not expressed a style preference in their options, or are attempting to use a style that does not exist or is forbidden.




- Variable Name: styleid
- Data Type: number
- Default Value: 1

## Allow Users To Change Styles

This allows users to set their preferred style set on registration or when editing their option. Setting this to 'No' disables that option and will force them to use whatever style has been specified.




- Variable Name: allowchangestyles
- Data Type: boolean
- Default Value: 1

## Store CSS Stylesheets and SVG Images as Files?

If you would like to store the CSS stylesheets and SVG Images for each style as a file, you must ensure that the directory set in the 'CSS and SVG File Location' option exists and that the web server has permission to write and delete files within that directory.




- Variable Name: storecssasfile
- Data Type: boolean
- Default Value: 

## CSS and SVG File Location

Relative path to CSS and SVG files.<br/>
The path relative to the core directory where you are storing the CSS and SVG files.<dfn>This only applies if you have set CSS as files. If empty it will default to cache/css</dfn>




- Variable Name: cssfilelocation
- Data Type: free
- Default Value: cache/css

## Show Instant Messaging Program Icons

Setting this option to yes will show the images for Skype, ICQ, AIM, MSN, and Yahoo! Messenger if the user has entered the correct information in his/her profile. These links are shown in various places throughout the forum, on posts, who's online, memberlist, profile, etc.




- Variable Name: showimicons
- Data Type: boolean
- Default Value: 1

## Use SkypeWeb Graphics

If set to 'Yes', load Skype&trade; icon from the SkypeWeb server in order to show users' online status, otherwise use local (static) graphic.<br />
<br />
If set to 'Language Specific', graphics in the language being used by the visiting user will be loaded.<br />
<br />
If the 'Language Specific' option does not work, switch it off and try again in a few weeks.




- Variable Name: skypeweb_gfx
- Data Type: number
- Default Value: 1

## Search Engine Referrers

Use this option to mark certain HTTP referrer addresses as a search engine source.<br />
<br />
Note that for most accurate detection (and save resource for checking similar things), you should enter only part of the domain.  For example, instead of entering "www.yahoo.com" and "www1.yahoo.com", enter just ".yahoo.com".  Instead of entering ".google.com", ".google.ca", ".google.co.uk", simply enter ".google.".<br />
<br />
Alternatively, if you only care about any part of the domain, you can use * as a wild card.  For example "search*" will match "searching.site", "searchmaster.site", etc.<br />
<br />
Put each search engine source on its own line.




- Variable Name: searchenginereferrers
- Data Type: free
- Default Value: .google.
.live.
.msn.
.yahoo.

## Cache Templates As Files

If this is selected the templates will be written as files in the directory selected.




- Variable Name: cache_templates_as_files
- Data Type: boolean
- Default Value: 0

## Template Cache Path

The location of the directory to store the compiled templates.  If the path is not absolute then it is interpreted as being relative to the vBulletin core directory.




- Variable Name: template_cache_path
- Data Type: free
- Default Value: cache/template


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>