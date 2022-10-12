---
Title: "Privacy Options"
Slug: privacy-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 50
---


## Enable Privacy Consent for Guests

This will require all users in the selected locations to consent to information tracking in order to use the site.  It will log the time the consent was given and the IP address the consent was obtained from.
You can edit the available locations <a href="admincp/locations.php?do=modify">here</a>.

<br /><br />If this is enabled, you must specify a Privacy Policy Page in the <a href="admincp/options.php?do=options&amp;dogroup=privacy#privacyurl">Privacy Statement URL</a> setting.




- Variable Name: enable_privacy_guest
- Data Type: free
- Default Value: 

## Enable Privacy Consent for Registered Users

This will collect consent for users in the selected locations when they register or the first time they log in (if they are already registered). You can edit the available locations <a href="admincp/locations.php?do=modify">here</a>.

<br /><br />If this is enabled, you must specify a Privacy Policy Page in the <a href="admincp/options.php?do=options&amp;dogroup=privacy#privacyurl">Privacy Statement URL</a> setting.




- Variable Name: enable_privacy_registered
- Data Type: free
- Default Value: 0

## Block Visitors

Visitors in the selected locations will be blocked and will be denied access to the forums. <br/><br/>

This setting will never block UNKNOWN users so, for it to have any effect, you must also specify a service in the <a href="admincp/options.php?do=options&amp;dogroup=privacy#geoip_provider">Geo IP Provider</a> setting below. You can edit the available locations <a href="admincp/locations.php?do=modify">here</a>.




- Variable Name: block_eu_visitors
- Data Type: free
- Default Value: 

## Privacy Statement URL

Enter the URL of your privacy statement, if you have one. Otherwise, leave this setting blank.

<br /><br />If you have <a href="admincp/options.php?do=options&amp;dogroup=privacy#enable_privacy_guest">Privacy Consent</a> enabled, you must specify a URL here. You may use the existing <a href="privacy" target="_blank">Privacy Policy Page</a>, enter its URL in this setting, and fill out your actual Privacy Policy in the "<a href="admincp/phrase.php?do=edit&amp;e[global][privacy_policy_page_text]">privacy_policy_page_text</a>" phrase.




- Variable Name: privacyurl
- Data Type: free
- Default Value: privacy

## Enable Automatic Account Deletion

Allow users to automatically withdraw consent to collect data and delete their accounts.  This will be done via a cron script after a "cool down" interval. You can edit the available locations <a href="admincp/locations.php?do=modify">here</a>.




- Variable Name: enable_account_removal
- Data Type: free
- Default Value: 

## Account Deletion Cooldown

Number of days before privacy consent withdrawal triggers the user removal.
After a user withdraws their privacy consent, they have this many days to change their mind before their user data is permanently removed.
This value must be greater than zero, but can be a decimal.
If "Enable Automatic Account Deletion" is disabled, this setting does nothing.




- Variable Name: user_autodelete_cooldown
- Data Type: number
- Default Value: 3

## Maximum Number of Users to Delete Per Run

When automated account deletion is enabled accounts will be deleted via scheduled task.  This setting affects the number of accounts deleted each time that script runs.  If accounts are not being deleted promptly, increasing this value may help.  However too large a value can cause the script to time out.




- Variable Name: user_autodelete_limit
- Data Type: integer
- Default Value: 3

## Geo IP Provider

The GeoIP provider will determine if a user is from the EU based on their IP address. If you do not select a GeoIP provider (or do not provide an application key if it's required) then all users will be treated as UNKNOWN users. UNKNOWN users will match any of the default locations but that can be changed <a href="admincp/locations.php?do=modify">here</a>.

For the "Block visitors" setting to have any effect, you need to explicitly set a provider here.




- Variable Name: geoip_provider
- Data Type: free
- Default Value: none

## GeoIP Service Key

This is the access key for the <a href='https://ipstack.com/'>IP stack GeoIP service</a>.  This is required to identify which users are affected by the EU regulations.




- Variable Name: geoip_service_key
- Data Type: free
- Default Value: 

## Guest Privacy Consent Cookie Name

Use this to specify the name of the cookie used by the guest privacy consent banner. Leave this blank to use the default of: COOKIE_PREFIX + "privacy_consent_guest".




- Variable Name: privacy_consent_cookie_name
- Data Type: free
- Default Value: 

## Delete Guest Privacy Consent Cookie on Logout

If set to "yes", the guest privacy consent cookie will be deleted along with all vBulletin cookies when a user logs out. This means that after they log out they will see the Guest Privacy Consent Banner again, provided that it is enabled.




- Variable Name: privacy_consent_delete_cookie
- Data Type: boolean
- Default Value: 0

## COPPA Registration System

Use the COPPA registration system. This complies with the COPPA laws and requires children under the age of 13 to get parental consent before they can post.<br />
<br />
For more info about this law, see here:
<a href="https://www.vbulletin.com/go/coppa" target="_blank">https://www.vbulletin.com/go/coppa</a>




- Variable Name: usecoppa
- Data Type: number
- Default Value: 0

## COPPA Registration System Cookie Check

This option will save a cookie onto the user's computer if an age  under 13 is entered.  Subsequent registration attempts will be failed, no matter what age is entered. This only applies if the previous option is set to either <em>Enable COPPA</em> or <em>Deny registration for users under 13 years</em>.




- Variable Name: checkcoppa
- Data Type: number
- Default Value: 1


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>