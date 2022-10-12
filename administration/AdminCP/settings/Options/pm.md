---
Title: "Private Messaging and vB Messenger Options"
Slug: private-messaging-and-vb-messenger-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 440
---


## Private Messaging Enabled

Turns the entire private messaging system on and off.




- Variable Name: enablepms
- Data Type: boolean
- Default Value: 1

## Instant Messaging Support - Check for New Private Messages

Selecting 'Yes' for this option will cause the system to check the private message database every time a user loads a page, and will display a visible prompt if a new message has just been saved.




- Variable Name: checknewpm
- Data Type: boolean
- Default Value: 1

## Maximum Messages Per-Page

This setting allows you to limit the number of messages users may display per page on the private messages folder view pages.<br />
<br />
<b>Note: </b>This number must be at least 1.




- Variable Name: pmmaxperpage
- Data Type: posint
- Default Value: 100

## Allow Message Icons for Private Messages

Allow the use of the standard message icons for private messages.




- Variable Name: privallowicons
- Data Type: boolean
- Default Value: 1

## Allow BB Code in Private Messages

Allow users to include BB code in their private messages? (Such as [b], [i] etc.)




- Variable Name: privallowbbcode
- Data Type: boolean
- Default Value: 1

## Allow Smilies in Private Messages

Allow users to include smilies in their Private Messages?




- Variable Name: privallowsmilies
- Data Type: boolean
- Default Value: 1

## Enable vB Messenger

Globally enable or disable vB Messenger. Enabling this enables the "Messages" header dropdown, initiating private messages from forum threads, and vB Messenger windows for private messaging.
See help for more info about vB Messenger.




- Variable Name: pmchat_enabled
- Data Type: boolean
- Default Value: 1

## vB Messenger Header Max

Maximum number of private messages to list in the header dropdown.<br />
<br />
<b>Note: </b>This number must be at least 1.




- Variable Name: pmchat_dropdown_max
- Data Type: posint
- Default Value: 6

## vB Messenger Header Polling Interval

Every X seconds (where X is the value set for this option), the client will send an ajax request to check for new private messages, notification & request counts for the header dropdown. <br />
Increase this setting to reduce server load. Decrease this setting for more frequent client side updates. <br />
<strong>Default:</strong> 30 seconds.




- Variable Name: pmchat_header_polling_interval
- Data Type: posint
- Default Value: 30

## vB Messenger Window Minimum Polling Interval

The Messenger window checks for new messages from the server in a dynamic fashion. <br />
When a new message is sent or retrieved, the Messenger window will temporarily go into a "burst" mode where it checks for new messages very quickly, but <strong>no faster than</strong> every X seconds (where X is the value of this setting). <br />
Increase this setting to reduce server load. Decrease this setting for a more responsive experience. <br />
<strong>Default:</strong> 1 second.




- Variable Name: pmchat_chat_polling_min_interval
- Data Type: posint
- Default Value: 1

## vB Messenger Window Maximum Polling Interval

The Messenger window checks for new messages from the server in a dynamic fashion. <br />
When no messages have been sent or received for a while, the Messenger window will ease into a "slow" mode where it checks for new messages only intermittently, but <strong>no slower than</strong> every X seconds (where X is the value of this setting). <br />
Increase this setting to reduce server load. Decrease this setting for a more responsive experience. <br />
This value should be greater than "<strong>vB Messenger Window Minimum Polling Interval</strong>". <br />
<strong>Default:</strong> 30 seconds.




- Variable Name: pmchat_chat_polling_max_interval
- Data Type: posint
- Default Value: 30

## vB Messenger Window Idle Timeout

When no new messages have been sent or received for X seconds (where X is the value of this setting), the Messenger window will go into "idle" mode and stop polling the server. The user can choose to resume polling by clicking a "Reconnect" button. <br />
Decrease this setting to reduce server load. <br />
This value should be greater than "<strong>vB Messenger Window Maximum Polling Interval
</strong>". <br />
<strong>Default:</strong> 300 seconds (5 minutes).




- Variable Name: pmchat_chat_polling_idle_timeout
- Data Type: posint
- Default Value: 300

## Minimum Characters Per Message

If this number is set to a value greater than 0, users must enter at least that number of characters in each new post.
<br /><br />
Set the value to 0 to disable this function.




- Variable Name: pmminchars
- Data Type: integer
- Default Value: 1

## Maximum Characters Per Message

Posts that contain more characters than the value specified here will be rejected with a message telling the user to shorten their post.<br />
<br />
Set the value to 0 to disable this function.




- Variable Name: pmmaxchars
- Data Type: integer
- Default Value: 10000

## Minimum Time Between Private Messages

You may prevent your users from flooding your private message center by activating this feature.

By enabling floodcheck, you disallow users from making another private message within a given time span of their last message. In other words, if you set a floodcheck time span of 30 seconds, a user may not create a private message topic or reply within 30 seconds of making his last message.

Administrators and moderators are exempt from floodcheck.

Recommended: 30 seconds. Type the number of seconds only. Enter 0 to disable this function.




- Variable Name: pm_floodchecktime
- Data Type: integer
- Default Value: 30

## Skip floodcheck for PM Replies

If enabled, the floodcheck is only applied to creating new private message threads. Replying to existing private message topics will be exempt from the floodcheck. This improves the user experience of vB Messenger as users will be able to create replies to each other very quickly in an existing private message thread.




- Variable Name: pm_floodcheck_starteronly
- Data Type: boolean
- Default Value: 0


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>