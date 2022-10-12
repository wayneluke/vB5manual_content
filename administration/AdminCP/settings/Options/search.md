---
Title: "Message Searching Options"
Slug: message-searching-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 370
---


## Search Engine Enabled

Allow searching for posts and topics within the forums. This is a relatively server-intensive process so you may want to disable it if you have problems.<br />
<br />
To disable searching of all forums, delete the option from the search_forums template.




- Variable Name: enablesearches
- Data Type: boolean
- Default Value: 1

## Minimum Time Between Searches

The minimum time (in seconds) that must expire before the user can perform a new search.<br />
<br />
Set this to 0 to allow users to search as frequently as they want.




- Variable Name: searchfloodtime
- Data Type: integer
- Default Value: 0

## Maximum Search Results to Return

Any search results over this number will be discarded.




- Variable Name: maxresults
- Data Type: integer
- Default Value: 500

## Search Index Minimum Word Length

This option limits the size of indexed words. The smaller this number is, the larger your search index, and conversely your database is going to be.<br /><br />
Other search implementations, such as Sphinx, use their own limits for words indexed, but this option still limits the size of words that may be searched.  Smaller words take longer to search for as they are more common.




- Variable Name: minsearchlength
- Data Type: integer
- Default Value: 4

## Search Index Maximum Word Length

This option limits the maximum size that of words that users can search for.
For example, if this is set to 15 then users can't search for 16 letter words.<br /><br />
When using the vBulletin default search, this option limits the maximum size of indexed words. The larger this number is, the larger your search index, and conversely your database is going to be.
You can reduce the size of your database by decreasing this number and re-indexing <a href="admincp/misc.php?do=chooser" target="_blank">here</a>.<br /><br />
Other search implementations, such as Sphinx, use their own limits for words indexed, but the searches will still be limited by this maximum size.





- Variable Name: maxsearchlength
- Data Type: integer
- Default Value: 20

## Words to be Included Despite Character Limit

If there are special words that are important for your forum but are outside the word length limits you specified in Message Searching Options, you may enter them here so that they will be included in the search index.<br />
<br />
For example, a web-programming forum with a minimum word length of 4 characters might want to include 'PHP' in the search index, even though the word is only 3 characters long.<br />
<br />
Separate each word with a space.




- Variable Name: goodwords
- Data Type: free
- Default Value: vb vbb php sql

## Words to be excluded from search

If there are special words that are very common for your forum, you may wish to remove them from being searchable.  Searching for very common words on a large forum can be server intensive.

Separate each word with a space.




- Variable Name: badwords
- Data Type: free
- Default Value: 

## Trending Lookback

Look back period for trending topics (in hours)<br/><br/>

Changes will take affect the next time the trending scheduled task runs.




- Variable Name: trendinglookback
- Data Type: integer
- Default Value: 96

## Trending Minimum Lifetime

Minimum lifetime for trending topics (in hours) <br/><br/>

Changes will take affect the next time the trending scheduled task runs.




- Variable Name: trendingminimum
- Data Type: integer
- Default Value: 4

## Max Event Duration

Upper limit of how long an event can last, in days.
<br />
Having this value too large will significantly impact search & calendar features.




- Variable Name: event_max_duration
- Data Type: posint
- Default Value: 31


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>