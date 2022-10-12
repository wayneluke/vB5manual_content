---
Title: "User Profile Options"
Slug: user-profile-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 210
---


## Require Date of Birth

Require users to provide a valid date of birth (1902 to current year).




- Variable Name: reqbirthday
- Data Type: boolean
- Default Value: 

## User Title Maximum Characters

This is the maximum number of characters allowed for a user's custom title.




- Variable Name: ctMaxChars
- Data Type: integer
- Default Value: 25

## Censored Words for Usertitle

Type all words you want censored in the Usertitle in the field below. Do not use commas to separate words, just use spaces. For example, type 'dog cat boy', rather than 'dog, cat, boy.'<br />
<br />
If you type 'dog', all words containing the string 'dog' would be censored (dogma, for instance, would appear as '***ma'). To censor more accurately, you can require that censors occur only for exact words. You can do this by placing a censor word in curly braces, as in {dog}. Signifying 'dog' in the curly braces would mean that dogma would appear as dogma, but dog would appear as '***'. Thus your censor list may appear as: cat {dog} {barn} barn<br />
<br />
Do not use quotation marks and make sure you use curly braces, not parentheses, when specifying exact words.




- Variable Name: ctCensorWords
- Data Type: free
- Default Value: admin forum moderator vbulletin leader

## Exempt Moderators From Censor

Do you want to exempt your forum Moderators from the censor words? You will want to set this to yes if you censor anything that is part of a moderator's title like 'moderator' as they have custom titles by default and will get censored.




- Variable Name: ctCensorMod
- Data Type: boolean
- Default Value: 1

## Number of friends to display in the small friends block

The Number of Friends to display in the Small Friends Block on the Users' Profile Pages




- Variable Name: minifriends_amount
- Data Type: integer
- Default Value: 6

## Signature Soft-Linebreak Character Limit

When counting the number of lines in a signature, this setting controls the number of characters that can be displayed before text wraps in the browser and is displayed as multiple lines. Once this value is surpassed, the run of text will be counted as multiple lines.<br />
<br />
The value in this setting should be based on the number of <em>normal-sized</em> characters. Other sized characters will be scaled appropriately to this setting.




- Variable Name: softlinebreakchars
- Data Type: integer
- Default Value: 90

## Allow Users to  'Ignore' Moderators

Allow users to add Moderators and Administrators to their ignore list?




- Variable Name: ignoremods
- Data Type: boolean
- Default Value: 

## Allow Signatures

This allows users to include a signature in their posts.




- Variable Name: allow_signatures
- Data Type: boolean
- Default Value: 1

## Enable User Profile Customization

Globally enable or disable user profile customization.




- Variable Name: enable_profile_styling
- Data Type: boolean
- Default Value: 1

## User Status Maximum Characters

This is the maximum number of characters allowed for a user's status, up to a hard limit of 1000 characters.




- Variable Name: statusMaxChars
- Data Type: integer
- Default Value: 140

## Use Namecards

If enabled, clicking on a username or display name with a profile link will pop-up a namecard instead of directly navigating to the profile page.




- Variable Name: usenamecard
- Data Type: boolean
- Default Value: 

## Allow Edit Display Names

If enabled, users will be able to change their own display names. If disabled, only admins will be able to edit users' display names.




- Variable Name: enabledisplayname
- Data Type: boolean
- Default Value: 

## Displayname Change Frequency

How many times per day a user is allowed to change their own display names. Edits via AdminCP will bypass this limit. Set it to 0 for no limit. <br />
Note, resetting the displayname back to their username is always allowed.




- Variable Name: displaynamechangefrequency
- Data Type: integer
- Default Value: 3


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>