---
Title: "Date and Time Options"
Slug: date-and-time-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 100
---


## Datestamp Display Option

This option controls the display of dates throughout your forum<br /><br />'Normal' uses the date and time formats below this option.<br />
<br />
'Yesterday / Today' will show 'Yesterday' and 'Today' for dates that fall in those periods.<br />
<br />
'Detailed' will show times such as '1 Minute Ago', '1 Hour Ago', '1 Day Ago', and '1 Week Ago'.




- Variable Name: yestoday
- Data Type: number
- Default Value: 1

## Default Time Zone Offset

Time zone offset for guests and new users. Do not take DST into consideration, rather use the next option to enable/disable DST.




- Variable Name: timeoffset
- Data Type: number
- Default Value: 

## Enable Daylight Savings

If Daylight Savings Time is currently in effect for the above time zone, enable this option so that guests will see the correct times on posts and events. This has no effect on registered users as they control their DST options in the User CP. 




- Variable Name: dstonoff
- Data Type: boolean
- Default Value: 

## Format For Date

Format in which the date is presented on vBulletin pages:<br />
<br />
See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a><br />
<br />
<b>Examples:</b><br />
US Format (e.g., 04-25-98): %d.%m.%Y<br />
Expanded US Format (e.g., April 25, 1998): %B %d, %Y<br />
European Format (e.g., 25-04-98): %d-%m-%y<br />
Expanded European Format (e.g., 25 April 1998): %d %B %Y




- Variable Name: dateformat
- Data Type: free
- Default Value: %m-%d-%Y

## Format For Time

Format in which the time is presented on all vBulletin pages:<br />
<br />
See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a><br />
<br />
<b>Examples:</b><br />
AM/PM Time Format (eg, 11:15 PM): %I:%M %p<br />
24-Hour Format Time (eg, 23:15): %H:%M




- Variable Name: timeformat
- Data Type: free
- Default Value: %I:%M %p

## Format For Registration Date

This is used to format the user's registration date, which is displayed in each user's post.<br />
<br />
See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a><br />




- Variable Name: registereddateformat
- Data Type: free
- Default Value: %b %Y

## Format For Birthdays with Year Specified

Format of date shown in profile when user gives their birth-year.

<br />
<br />
See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a><br />




- Variable Name: calformat1
- Data Type: free
- Default Value: %B %d, %Y

## Format For Birthdays with Year Unspecified

Format of user's birthday shown on profile when the user does not specify their birth-year.<br />
<i>DO NOT put in a code for the year.</i>

<br />
<br />
See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a>




- Variable Name: calformat2
- Data Type: free
- Default Value: %B %d

## Format for Event Dates in the Upcoming Events Module

This is the format for the event start date as shown in the Upcoming Events module. You only need to enter the format for month and day, since there is a separate year header in the module.

<br />
<br />
See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a>




- Variable Name: eventdateformat
- Data Type: free
- Default Value: %b %d

## Format for DateTime Picker

This is the format for the date and time as shown in the DateTime Picker. Enter formatting codes for the date and the time.

<br /><br />See: <a href="https://flatpickr.js.org/formatting/" target="_blank">https://flatpickr.js.org/formatting/</a>




- Variable Name: pickerdateformat
- Data Type: free
- Default Value: n-j-Y h:i K

## Log Date Format

Format of dates shown in Control Panel logs.<br /><br />See: <a href="admincp/diagnostic.php?do=displaydateformat" target="_blank">here</a><br />




- Variable Name: logdateformat
- Data Type: free
- Default Value: %H:%M, %d %b %Y


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>