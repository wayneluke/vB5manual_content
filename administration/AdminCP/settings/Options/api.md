---
Title: "vBulletin API and Mobile Application Options"
Slug: vbulletin-api-and-mobile-application-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 1010
---


## Enable vBulletin API

Allow clients to connect to the vBulletin API. <br /><br />Please remember to generate an API key <a href="admincp/api.php">here</a> to allow the API to work.




- Variable Name: enableapi
- Data Type: boolean
- Default Value: 0

## Enable API Log

Enables the API log, allowing administrators to track client behavior (or for debuging purposes). Only enable this option if you really need it. The log is stored in the database and can rapidly become large in size.




- Variable Name: enableapilog
- Data Type: boolean
- Default Value: 0

## Log API POST parameters

When "Enable API Log" is set to "Yes", this option decides whether to log API POST parameters. Please note that POST parameters can contain a lot of data, which can in turn can take up large amounts of database space.




- Variable Name: apilogpostparam
- Data Type: boolean
- Default Value: 0

## Enable Firebase Cloud Messaging

Enabling this option will allow mobile api users to register their devices with the forum and receive push notifications via Firebase Cloud Messaging.
In addition to this option, the server must have a valid "Firebase Cloud Messaging Server Key" below for push notifications to function.




- Variable Name: fcm_enabled
- Data Type: boolean
- Default Value: 1

## Firebase Cloud Messaging Server Key

This is the "Server key" found in the "Cloud Messaging" Tab of your Firebase Cloud Messaging project. <br />
You can get to this tab via (as of 2017-05-18)
https://console.firebase.google.com/project/{projectid}/settings/cloudmessaging/
Where {projectid} is the unique id assigned to your firebase project. <br />
<br />
After you save this option, you can test the server key <a href="admincp/fcm.php">here</a>.




- Variable Name: fcm_serverkey
- Data Type: free
- Default Value: 

## Firebase Cloud Messaging Offload Timeout

This option specifies the max time (in seconds) the system will wait for a response from the child thread that handles communications with the Firebase Cloud Messaging before timing out and discarding the notification attempt. 
<br />
Increase this value only if push notifications are not being sent out reliably.




- Variable Name: fcm_worker_remote_timeout
- Data Type: posint
- Default Value: 3

## MAPI Activity Content Types

Content types to show in the mobile activity stream.




- Variable Name: mapi_activity_type
- Data Type: free
- Default Value: [&quot;vBForum_Text&quot;,&quot;vBForum_Gallery&quot;,&quot;vBForum_Video&quot;,&quot;vBForum_Link&quot;,&quot;vBForum_Poll&quot;,&quot;vBForum_Event&quot;]

## MAPI Activity Topics Only

If yes, only topics will be displayed in the mobile activity stream.




- Variable Name: mapi_activity_starter_only
- Data Type: boolean
- Default Value: 0

## MAPI Activity Results per Page

Number of results per page for mobile activity stream.




- Variable Name: mapi_activity_per_page
- Data Type: integer
- Default Value: 15

## MAPI Activity Date Range

Only results from the last specified range will be returned by the mobile activity stream.




- Variable Name: mapi_activity_date_range
- Data Type: free
- Default Value: lastMonth


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>