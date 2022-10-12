---
Title: "Admin Control Panel Options"
Slug: admin-control-panel-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 520
---


## Control Panel Style Folder

This setting allows you to specify an alternative style for the Admin / Moderator Control Panels, based on a folder contained within the 'cpstyles' folder. The style you select here will be displayed to all Moderators, and any Administrators who have not expressed their own preference.<br />
<br />
Folders in the 'cpstyles' folder must contain at least the following:<br />
<br />
- controlpanel.css<br />
- cp_logo.gif<br />
- cp_help.gif




- Variable Name: cpstylefolder
- Data Type: free
- Default Value: vBulletin_5_Default

## Control Panel Style Image Extension

Choose the file extension for the images used by your Control Panel Style.




- Variable Name: cpstyleimageext
- Data Type: free
- Default Value: png

## Timeout Admin Login

After a period of inactivity, Administrators are logged out of the Admin Control Panel.  If this option is set to yes, the inactivity period will be the same as the Cookie Timeout setting found in vBulletin Options -> Help Cookies and HTTP Header Options (defaults to 15 minutes).  If this option is disabled, then the period will be one hour.
<br /><br />Logins to the admincp are more secure with this enabled.




- Variable Name: timeoutcontrolpanel
- Data Type: boolean
- Default Value: 

## Control Panel Quick Statistics

Display additional 'Quick Stats' on the main index page of the Admin Control Panel? Displaying these statistics may cause a performance issue on large boards.




- Variable Name: adminquickstats
- Data Type: boolean
- Default Value: 

## Forum Manager Display

There are three options for the display of the Forum Manager:<br />
<ul>
	<li><span class="smallfont"><i>Default</i> - Displays all of the forums on one page but may not work on all browsers, especially if you have a large number of forums.</span></li>
	<li><span class="smallfont"><i>Collapsible</i> - Allows collapsing/expansion of certain forums within the forum manager.  This may reduce the ease of usability of the forum manager, but will prevent rendering problems with the dropdown menus with certain browsers/operating systems.</span></li>
	<li><span class="smallfont"><i>Single</i> - Display a single dropdown from which you may choose the forum you wish to modify. This is most useful if you have a large number of forums.</span></li>
</ul>




- Variable Name: cp_collapse_forums
- Data Type: number
- Default Value: 

## User Editor Columns

Number of columns to display in user editor. Smaller resolutions will probably want to set this to 1.




- Variable Name: cp_usereditcolumns
- Data Type: number
- Default Value: 2


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>