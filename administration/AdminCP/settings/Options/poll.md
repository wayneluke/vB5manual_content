---
Title: "Poll and Topic Rating Options"
Slug: poll-and-topic-rating-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 360
---


## Maximum Poll Options

Maximum number of options a user can select for the poll.<br />
<br />
Set this option to 0 to allow any number of options.




- Variable Name: maxpolloptions
- Data Type: integer
- Default Value: 10

## Initial Poll Options

The number of options displayed by default when a new poll is created.  The actual values displayed will not be less than two or greater than Max Poll Options.




- Variable Name: initialpolloptions
- Data Type: integer
- Default Value: 3

## Poll Option Length

Maximum length that a poll option can be.




- Variable Name: maxpolllength
- Data Type: integer
- Default Value: 100

## Update Topic Last Post on Poll Vote

If you set this option to 'Yes' the topic's last post time will be updated when a vote is placed, thereby returning it to the top of its parent forum listing.<br />
<br />
Note that this option can cause confusion. The last post time of a topic will be changed with no visible post.




- Variable Name: updatelastpost
- Data Type: boolean
- Default Value: 

## Required Topic Rating Votes to Show Rating

This option specifies the number of topic rating votes that must be cast of a particular topic before the current rating is displayed on forumdisplay.php and showthread.php.




- Variable Name: showvotes
- Data Type: integer
- Default Value: 1

## Allow Topic Rating Vote Changes

Allow users to change their original rating of a topic?




- Variable Name: votechange
- Data Type: boolean
- Default Value: 


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>