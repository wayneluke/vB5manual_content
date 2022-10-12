---
Title: "User Profile: Album Options"
Slug: user-profile-album-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 215
---


## Albums Per Page

When listing multiple albums on one page, this controls how many will be displayed before pagination occurs.<br />
<br />
<b>Note: </b>This number must be at least 1.




- Variable Name: albums_perpage
- Data Type: posint
- Default Value: 10

## Pictures Per Page

When viewing an album, this controls how many pictures are displayed before pagination occurs.<br />
<br />
<b>Note: </b>This number must be at least 1.




- Variable Name: album_pictures_perpage
- Data Type: posint
- Default Value: 25

## Number of Albums to display in the Users Profile

The Maximum Number of Albums to Display on the Users' Profile Pages




- Variable Name: profile_album_amount
- Data Type: integer
- Default Value: 2

## Picture Moderation

When enabled, all new pictures are placed into moderation. This can also be enabled in usergroup permissions.




- Variable Name: albums_pictures_moderation
- Data Type: boolean
- Default Value: 0

## Caption Preview Length

The amount of characters from a picture's caption that will be shown when a user hovers over the picture.




- Variable Name: album_captionpreviewlen
- Data Type: integer
- Default Value: 150

## Maximum Pictures per Album

You may choose to limit the number of pictures that a user can have in one album. This is primarily useful for encouraging your users to have albums for smaller topics, but it does have minor performance considerations as well. The usergroup setting "Maximum Number of Album Pictures" takes precedence over this setting.<br />
<br />
Set this to 0 to disable the limit.




- Variable Name: album_maxpicsperalbum
- Data Type: integer
- Default Value: 60

## Enable Picture Comments

Set this option to yes if you would like to enable commenting on album and group pictures. Comments are associated with the picture itself, so comments will be shown anywhere the picture is shown.




- Variable Name: pc_enabled
- Data Type: boolean
- Default Value: 1

## Moderate Picture Comments

When enabled, all new picture comments are placed into moderation. This can also be enabled in usergroup permissions.




- Variable Name: pc_moderation
- Data Type: boolean
- Default Value: 0

## Default Picture Comments Per-Page

This setting allows you to define the default number of picture comments displayed per-page with a picture.<br />
<br />
<b>Note: </b>This number must be at least 1.




- Variable Name: pc_perpage
- Data Type: posint
- Default Value: 10

## Maximum Picture Comments Per-Page

This setting allows you to limit the number of picture comments users may display per page with a picture.<br />
<br />
<b>Note: </b>This number must be at least 1.




- Variable Name: pc_maxperpage
- Data Type: posint
- Default Value: 50

## Allowed BB Code Tags in Picture Comments

This setting allows you to enable and disable  the use of various BB codes in picture comments.<br />
<br />
Note that any changes you make will only affect messages posted (or edited) after this point.




- Variable Name: pc_allowed_bbcode
- Data Type: bitfield
- Default Value: 1091


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>