---
Title: "Facebook Options"
Slug: facebook-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 60
---


## Enable Facebook Platform

Enabling this option will allow users to connect their vBulletin account with their Facebook account. This will also populate your site with Open Graph meta data. Note: users must have Javascript enabled and your server must support TLS/SSL communication for this feature to work.




- Variable Name: enablefacebookconnect
- Data Type: boolean
- Default Value: 0

## Facebook Application ID

Enter the Application ID for your Application (see the <a href="http://www.facebook.com/developers/" target="_blank">Facebook Developer</a> page for more information).




- Variable Name: facebookappid
- Data Type: free
- Default Value: 

## Facebook Secret

Enter the Facebook Secret for your Application (see the <a href="http://www.facebook.com/developers/" target="_blank">Facebook Developer</a> page for more information).




- Variable Name: facebooksecret
- Data Type: free
- Default Value: 

## Facebook Usergroup

If you want, you may specify a secondary usergroup for Facebook users. Note: All users who connect with facebook from this point on will be members of this usergroup. This will not be applied retroactively to users who have previously connected to facebook.




- Variable Name: facebookusergroupid
- Data Type: number
- Default Value: 

## Enable Quick Register

This option will present the user with a simplified registration form when they register by clicking the Facebook Icon in the login box.<br/><br/>

Note: This feature will disable some of the normal registration checks.




- Variable Name: facebookautoregister
- Data Type: boolean
- Default Value: 0

## Image URL

Specify a URL for an image that you want to represent your site. This image will appear next to published content in a user's newsfeed, as well as be used to represent your site in the Open Graph schema. Leave this blank if you do not want to have an image.<br/><br/>

This  must be a fully qualified URL.




- Variable Name: facebookfeedimageurl
- Data Type: free
- Default Value: 

## Show Open Graph Meta Tags

vBulletin sets some information about the site in html header tags that Facebook and other social media sites use when people link to your site.  Usually you want these, but if you have a custom solution that implements these tags, you should turn them off to avoid conflicts.




- Variable Name: show_opengraph_tags
- Data Type: boolean
- Default Value: 1


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>