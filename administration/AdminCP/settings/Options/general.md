---
Title: "General Settings"
Slug: general-settings
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 30
---


## Login Credential Type

This option lets users log in using only their email, only their username, or both.




- Variable Name: logintype
- Data Type: number
- Default Value: 1

## Use Login "Strikes" System

Setting this to no will disable the system that prevents a user (with a specific IP address) from logging into an account after entering an incorrect password 5 times.




- Variable Name: usestrikesystem
- Data Type: boolean
- Default Value: 1

## Post Referrer Whitelist

For security purposes, vBulletin only allows data to be submitted via post from within the domain the board is installed on. If you are submitting post requests from a different domain or subdomain, you must add them here.
<br /><br />
Enter domains in the form of .domain.com (including the leading dot). Separate multiple domains by line breaks.




- Variable Name: allowedreferrers
- Data Type: free
- Default Value: 

## Topic/Forum Read Marking Type

This option controls how topics and forums are marked as read.<br />
<br />
Click the help icon on the right for more information on each option.




- Variable Name: threadmarking
- Data Type: free
- Default Value: 2

## Database Read Marking Limit

The amount of time in days to store the topic and forum read times. All topics or forums without posts in this many days will be considered read.




- Variable Name: markinglimit
- Data Type: number
- Default Value: 10

## Enable Inline Moderation Authentication

Inline moderation actions will require a user to authenticate again prior to being performed. The timeout is based on the admin control panel timeout, or one hour if that option is disabled.




- Variable Name: enable_inlinemod_auth
- Data Type: boolean
- Default Value: 1

## Disable Static HTML and Ad Module rendering

In order to fix an error with Static HTML or Ad module errors, you may need to temporary disable rendering for these modules.




- Variable Name: disable_php_rendering
- Data Type: boolean
- Default Value: 

## Number of Pages Visible in Page Navigator

If a thread/forum (etc.) requires multiple pages to be displayed, this option selects how many page links either side of the current page are shown. Set this to 0 to display all pages.




- Variable Name: pagenavpages
- Data Type: number
- Default Value: 3

## Relative Jumps for Page Navigator

If a thread/forum (etc.) requires multiple pages to be displayed, this option selects what pages can be jumped to relative to the current one. For example, by adding 10 to the list, links will appear for current page -10 and current page +10.




- Variable Name: pagenavs
- Data Type: free
- Default Value: 10 50 100 500 1000


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>