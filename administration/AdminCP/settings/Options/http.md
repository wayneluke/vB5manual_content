---
Title: "Cookies and HTTP Header Options"
Slug: cookies-and-http-header-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 110
---


## Session Timeout

This is the time in seconds that a user must remain inactive before their login session expires. This setting also controls how long a user will remain on Who's Online after their last activity.




- Variable Name: cookietimeout
- Data Type: integer
- Default Value: 900

## GZIP HTML Output

Selecting yes will enable vBulletin to GZIP compress the HTML output of pages, thus reducing bandwidth requirements. This will be only used on clients that support it, and are HTTP 1.1 compliant. There will be a small performance overhead.<br />
<br />
This feature requires the ZLIB library.<br />
<br />
If you are already using <b>mod_gzip</b> or <b>mod_deflate</b> on your server, do not enable this option.




- Variable Name: gzipoutput
- Data Type: boolean
- Default Value: 0

## GZIP Compression Level

Set the level of GZIP compression that will take place on the output. 0=none; 9=max.<br />
<br />
We strongly recommend that you use level 1 for optimum results.




- Variable Name: gziplevel
- Data Type: number
- Default Value: 1

## Add Standard HTTP Headers

This option does not work with some combinations of web server, so it is off by default. However, some IIS setups may need it turned on.<br />
<br />
It will send the 200 OK HTTP headers if turned on.




- Variable Name: addheaders
- Data Type: boolean
- Default Value: 

## Add No-Cache HTTP Headers

Selecting yes will cause vBulletin to add no-cache HTTP headers. These are very effective, so adding them may cause server load to increase due to an increase in page requests.




- Variable Name: nocacheheaders
- Data Type: boolean
- Default Value: 

## Cache time for permanent redirects

This is the lifetime (in days) that permanent redirects are cached.




- Variable Name: 301cachelifetime
- Data Type: number
- Default Value: 2

## Anti Clickjacking Headers

This setting allows you to turn on HTTP headers to help mitigate <em>Clickjacking</em> and <em>UI Redress</em> attacks by preventing your vBulletin site from being loaded inside a &lt;frame&gt; or similar element by an attacker.

<br /><br />If enabled, this sends <em>X-Frame-Options</em> and <em>Content-Security-Policy</em> headers.




- Variable Name: clickjackingheaders
- Data Type: integer
- Default Value: 2

## Content-Security-Policy Header

Use this option to set the the content for the  <code>Content-Security-Policy</code> header. You can find information about this header and its possible values here: <a href="https://developer.mozilla.org/en-US/docs/Web/HTTP/Headers/Content-Security-Policy" target="_blank">Content-Security-Policy</a>.

<br /><br />Any <code>frame-ancestors</code> directives in this header may be modified to ensure that certain vBulletin pages that use frames, such as the Admin CP and login form, will continue to work. 

<br /><br />If you deny or limit framing in the <b>Anti Clickjacking Headers</b> setting, it may conflict with <code>frame-ancestors</code> directives here.




- Variable Name: header_contentsecuritypolicy
- Data Type: free
- Default Value: 


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>