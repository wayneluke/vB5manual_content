---
Title: "Channel Display Options"
Slug: channel-display-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 420
---


## Show Private Forums

Select 'No' here will hide private forums from users who are not allowed to access them. Users who do have permission to access them will have to log in before they can see these forums too.<br />
<br />
This option applies to any forum listing, including the Quick Navigation menu, and Search Results.




- Variable Name: showprivateforums
- Data Type: free
- Default Value: 0

## Show Topic Prefix in Last Post Column?

You may choose to show a topic's prefix in the last post column, along with the title. This will increase the size of the data included in that column, however.




- Variable Name: showprefixlastpost
- Data Type: number
- Default Value: 2

## Show Sticky Topics on All Pages

Select 'Yes' to show sticky topics on every forumdisplay.php page, regardless of page number. Set 'No' to only display them on page one.




- Variable Name: showstickies
- Data Type: boolean
- Default Value: 0

## Highlight Topics in Which User Has Posted

When this feature is enabled, a logged in user will see an 'arrow' (or whatever graphic you choose) on the folder icons (hot folders, new folders, etc.) next to the topics that they have posted in.




- Variable Name: showdots
- Data Type: boolean
- Default Value: 1

## Length of Topic Preview Text

This setting allows you to specify how many characters of the first post in a topic to display in the 'title' tag of the topic title on the forumdisplay page.<br />
<br />
Set this value to 0 to disable topic previews.




- Variable Name: threadpreview
- Data Type: integer
- Default Value: 150

## Age of Channel Display Last Content

For the channel listings this set the maximum age, in minutes, of the channel "last content" data. We recommend this be set to at least a minute and preferably five minutes. You can disable caching by setting to zero, but this will significantly increase server load.




- Variable Name: channeltreelife
- Data Type: integer
- Default Value: 1

## Use Avatars as Topic Status Icons

This will show the topic starter's avatar by the title of the topic when viewing the channel. If this is disabled, the topic status icons will be shown instead.




- Variable Name: avatarintopiclist
- Data Type: boolean
- Default Value: 0

## Default Article Preview Length in Characters

By default, this many characters from the beginning of an article will be displayed for the preview. You can change this for an individual article by setting the previewbreak in the editor.




- Variable Name: def_cms_previewlength
- Data Type: posint
- Default Value: 500

## Article Preview Image Size

When you create a Text article, the first image attachment found will be used to generate a preview image shown in the category. This setting determines the size for that preview image.<br /><br />Available sizes are determined by the <a href="admincp/options.php?do=options&amp;dogroup=attachment#attachresizes">Attachment Resize Options</a>.




- Variable Name: cmspreviewimagesize
- Data Type: free
- Default Value: thumb

## Default Blog Page Template

Specify the default page template to use for blogs




- Variable Name: blog_pagetemplate
- Data Type: number
- Default Value: 


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>