---
Title: "BB Code Settings"
Slug: bb-code-settings
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 300
---


## Enabled Built-in BB Code Tags

This setting allows you to enable and disable various built-in BB code tags in vBulletin.<br />
<br />
Disabling a BB code tag will prevent it from working anywhere on the forum, including signatures, private messages, user notes etc.
Disabling Video & Image BB codes will also disable the video & image ckeditor buttons, respectively. Disabling Image BB Code will also disable inline image attachment rendering.




- Variable Name: allowedbbcodes
- Data Type: bitfield
- Default Value: 59391

## Maximum [CODE] Lines

When a user posts a block of [CODE], [PHP] or [HTML] in one of their messages, the system will place it in a box, which expands to contain their message.<br />
<br />
This value controls the number of lines at which the box stops adding height and inserts a scrollbar.




- Variable Name: codemaxlines
- Data Type: integer
- Default Value: 30

## Allow BB Code in Non Forum Specific Areas

Allow users to include BB code in non-forum-specific areas? (Such as [b], [i] etc.)




- Variable Name: allowbbcode
- Data Type: boolean
- Default Value: 1

## Allow Smilies in Non Forum Specific Areas

Allow users to include smilies in Non Forum Specific Areas?




- Variable Name: allowsmilies
- Data Type: boolean
- Default Value: 1

## Allow [IMG] Code in Non Forum Specific Areas

Allow users to include [IMG] codes in Non Forum Specific Areas?




- Variable Name: allowbbimagecode
- Data Type: boolean
- Default Value: 

## Allow HTML in Non Forum Specific Areas

Allow users to include raw HTML code in Non Forum Specific Areas?<br />(<b>Strongly not recommended.</b>)




- Variable Name: allowhtml
- Data Type: boolean
- Default Value: 

## Add nofollow attribute to URL BB Code

If enabled rel="nofollow" will be added to the any anchor tags for an external resource outputted from the URL BB Code.




- Variable Name: url_nofollow
- Data Type: boolean
- Default Value: 0

## URL nofollow domain Whitelist

This setting specifies the domains which will be exempt from the nofollow attribute being added to outgoing links. Place each domain on a new line <strong>without</strong> the http://




- Variable Name: url_nofollow_whitelist
- Data Type: free
- Default Value: 

## Allow remote [video] retrieval

The display of certain provider's video using the [video] tag requires a remote request to be sent to the video service in order to retrieve the video page. Though this is only performed when the video is submitted with a post, you may wish to disable this ability. This option determines how many remote retrievals will be allowed with a single post submission. Set this option to 0 to disable remote retrieval.




- Variable Name: bbcode_video_scrape
- Data Type: integer
- Default Value: 3

## WMODE Setting

Choose the desired wmode setting for playback of embedded flash videos.




- Variable Name: player_wmode
- Data Type: free
- Default Value: opaque

## Display Avatars Next to @User Mentions

If set to "Yes", user avatars will be displayed next to @user mentions or instances of the [USER] bbcode in posts.




- Variable Name: userbbcodeavatar
- Data Type: boolean
- Default Value: 1

## Cache BBCode Render by Usergroup

This will cache rendered BBCode text per usergroup instead caching the same value for all users.  This is only needed if you have customizations to the BBCode templates that depend on usergroups or permissions.  This option can reduce the effectiveness of the cache.




- Variable Name: cachebbcodebyusergroup
- Data Type: boolean
- Default Value: 0


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>