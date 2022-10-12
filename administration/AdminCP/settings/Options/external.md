---
Title: "External Data Provider"
Slug: external-data-provider
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 530
---


## Enable External Javascript

This setting allows you to enable/disable the Javascript content syndication system that allows you to embed vBulletin data in HTML pages.




- Variable Name: externaljs
- Data Type: boolean
- Default Value: 

## Enable RSS Syndication

This setting allows you to enable/disable the RSS content syndication system.




- Variable Name: externalrss
- Data Type: boolean
- Default Value: 

## Enable XML Syndication

This setting allows you to enable/disable the XML content syndication system.




- Variable Name: externalxml
- Data Type: boolean
- Default Value: 

## Topic Cutoff

This value controls how many days in the past that updated topics will be chosen from.  Busy forums will want a smaller number. The smallest valid value is 1 day; the default is 30 days.




- Variable Name: externalcutoff
- Data Type: number
- Default Value: 30

## Topic Cache Lifespan

This setting controls how long topic content will be cached (in minutes). Valid settings are 1 to 1440, anything else will be treated as the default value of 60. The higher this value is, the less resources will be used by the External Data Provider system.




- Variable Name: externalcache
- Data Type: number
- Default Value: 60

## Maximum External Records

This option limits the maximum amount of records that can be returned by the external data provider.  By default 15 records will be returned. This option allows the user to tack on &amp;count=X to their RSS feed to retrieve more records.




- Variable Name: externalcount
- Data Type: integer
- Default Value: 15


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>