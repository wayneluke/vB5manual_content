---
Title: "User Registration Options"
Slug: user-registration-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 200
---


## Allow New User Registrations

Set this option to NO if you would like to temporarily (or permanently) prevent anyone new from registering. Anyone attempting to register will be told that you are not accepting new registrations at this time.




- Variable Name: allowregistration
- Data Type: boolean
- Default Value: 1

## Paid Subscription during Registration

Allow you to set the paid subscription as a required field during registration that new members need to select a paid subscription and pay before becoming a member.




- Variable Name: regrequirepaidsub
- Data Type: boolean
- Default Value: 

## Moderate New Members

Allows you to validate new members before they are classified as registered members and are allowed to post.




- Variable Name: moderatenewmembers
- Data Type: boolean
- Default Value: 

## Send Welcome Email

Enabling this option will send a welcome email to new users. To alter or translate this email, use the following links:<br /><br /> [<a href="admincp/phrase.php?do=edit&amp;e[emailsubject][welcomemail_gemailsubject]" target="_blank">Email Title</a>] [<a href="admincp/phrase.php?do=edit&amp;e[emailbody][welcomemail_gemailbody]" target="_blank">Email Body</a>]<br />
<br />
Note: If you require emails to be verified, this email will be sent after the user has activated his or her account. If you moderate new memberships, no welcome mail will be sent as the user will already be receiving an email.




- Variable Name: welcomemail
- Data Type: boolean
- Default Value: 1

## Welcome Private Message

Please input the username of the user that this PM is to be sent from. If no username is set then the Welcome PM will not be sent.<br /><br />

To alter or translate this message, use the following links:<br /><br /> [<a href="admincp/phrase.php?do=edit&amp;e[emailsubject][welcomepm_gemailsubject]" target="_blank">PM Title</a>] [<a href="admincp/phrase.php?do=edit&amp;e[emailbody][welcomepm_gemailbody]" target="_blank">PM Body</a>]<br />
<br />
Note: If you require emails to be verified, this message will be sent after the user has activated his or her account. Also ensure that <em>Receive Private Messages</em> is enabled in <strong>Default Registration Options</strong> below.




- Variable Name: welcomepm
- Data Type: username
- Default Value: 

## Email Address to Notify About New Members

This email address will receive an email message when a new user signs up. Leave the option blank to disable this function.




- Variable Name: newuseremail
- Data Type: free
- Default Value: 

## Allow Multiple Registrations Per User

Normally, vBulletin will stop users signing up for multiple names by checking for a cookie on the user's machine. If one exists, then the user may not sign up for additional names. <b>Note</b>: This does not stop users from logging out and then registering new accounts.<br />
<br />
If you wish to allow your users to sign up for multiple names, then select yes for this option, and they will not be blocked from registering additional usernames.




- Variable Name: allowmultiregs
- Data Type: boolean
- Default Value: 

## Verify Email Address in Registration

If you set this option to 'Yes' new members will not be allowed to post messages until they visit a link that is sent to them in an email when they sign up.<br />
<br />
If a user's account is not activated by the user visiting the link, it will remain in the 'Users Awaiting Activation' usergroup.




- Variable Name: verifyemail
- Data Type: boolean
- Default Value: 

## Require Unique Email Addresses

The default option is to require unique email addresses for each registered user. This means that no two users can have the same email address. You can disable this requirement by setting this option to 'No'.




- Variable Name: requireuniqueemail
- Data Type: boolean
- Default Value: 1

## Minimum Username Length

Enter the minimum number of characters in a valid username, for the purpose of ensuring that new members create valid usernames.




- Variable Name: minuserlength
- Data Type: integer
- Default Value: 3

## Maximum Username Length

Enter the maximum number of characters in a valid username, for the purpose of ensuring that new members create valid usernames.




- Variable Name: maxuserlength
- Data Type: integer
- Default Value: 25

## Illegal User Names

Enter names in here that you do not want people to be able to register.<br />
<br />
If any of the names here are included within the username, the user will be told that there is an error. For example, if you make the name <b>John</b> illegal, the name <b>John</b>athan will also be disallowed.<br />
<br />
Separate names by spaces.




- Variable Name: illegalusernames
- Data Type: free
- Default Value: 

## Username Regular Expression

You may require the username to match a regular expression (<a href="http://www.php.net/manual-lookup.php?function=preg-match" target="_blank">PCRE</a>).  The admin help provides some examples that may be useful. To disable this function leave the option blank.




- Variable Name: usernameregex
- Data Type: free
- Default Value: 

## Username Reuse Delay

When a username is changed, you may wish to prevent users from registering with that name for a certain length of time.<br />
<br />
Enter the number of days which an old username is reserved for. (Use 0 to disable.)




- Variable Name: usernamereusedelay
- Data Type: integer
- Default Value: 365

## Default Registration Options

The user options on the New User creation form in the Admin Control Panel, as well as the New User registration form will default to the following settings.




- Variable Name: defaultregoptions
- Data Type: bitfield
- Default Value: 717718665

## Minimum Password Length

When users create an account or change their password, they will be required to create a password that is at least this many characters long.




- Variable Name: passwordminlength
- Data Type: posint
- Default Value: 8

## Disallowed Password Words

You may add common words and commonly used and known passwords to this list. Please place each word on its own line. These words are not case sensitive. Any word included on this list will not be allowed as a password when users register or change their password. If the user's password merely contains one of these words it will still be allowed. For example, if you include "horse" in this list, then the password "horse" or "Horse" will be disallowed, but the password "CorrectHorseBatteryStaple" will be allowed.




- Variable Name: passwordbadwords
- Data Type: free
- Default Value: 

## Require Uppercase in Passwords

If enabled, users will be required to use at least one uppercase letter in their password.




- Variable Name: passwordrequireuppercase
- Data Type: boolean
- Default Value: 0

## Require Numbers in Passwords

If enabled, users will be required to use at least one number in their password.




- Variable Name: passwordrequirenumbers
- Data Type: boolean
- Default Value: 0

## Require Special Characters in Passwords

If enabled, users will be required to use at least one puncuation mark or other special character in their password.




- Variable Name: passwordrequirespecialchars
- Data Type: boolean
- Default Value: 0

## User Referral Code Expiration

This setting controls the number of days that a user referral code is valid. Users can generate a referral link to refer friends to the forums on their user profile page, if they are a member of a usergroup that permits referrals via the "Can Refer Users" permission.




- Variable Name: user_referral_expire_days
- Data Type: posint
- Default Value: 30


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>