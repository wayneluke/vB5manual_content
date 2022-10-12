---
title: "System Requirements"
slug: "system_requirements"
weight: 10
categories: 
- "getting_started"
tags: 
- beginner
- getting_started
---

Your server must meet the following requirements before vBulletin can be installed on the machine. Most shared-environment hosting providers meet these qualifications already. If you're unsure, you can always use [vBulletin Cloud](http://www.vbulletin.com/en/vbulletin-cloud/) to host your vBulletin website.

## Minimum Requirements
vBulletin is a web-based application and as such has a few minimum requirements. To run vBulletin, you need a web hosting provider that includes the following on their systems:
- PHP version: 7.4.0
- MySQL version: 5.7
    - As an alternative to MySQL, you can use MariaDB version 10.3. 
- A pre-registered domain name
- 200 Megabytes of hard drive space
- Rewrite Engine – A rewrite engine is needed for vBulletin's Friendly URL routing to work. Popular rewrite engines include mod_rewrite on Apache 2.4+ and "URL Rewrite" for IIS 7+.
- MySQLi support – MySQLi is a more robust software library to connect to the database that vBulletin uses.
- mbstring library - A PHP library that helps with character conversion for UTF-8 support.
- iconv library – A PHP library that provides extra language and character set support.


## Recommended Requirements
The following settings and software packages are not required but will make your vBulletin experience more enjoyable. Your hosting provider can tell you whether these are available on your server.
- PHP 8.0 or higher.
- MySQL 8.0 or greater.
- cURL or OpenSSL support – Allows secure connections to third-party services like Facebook Connect.
- OpCode Cache – An OpCode Cache like APC or XCache will enhance the performance of your vBulletin software. An OpCode Cache is a caching mechanism that can significantly increase the performance of vBulletin by pre-parsing the PHP files and keeping commonly used data in memory for rapid retrieval.

## Sphinx Search
A minimum version of Sphinx 2.4.2 is required to use Sphinx Search instead of MySQL for keyword based searches.

## Browser Support

- Chromium-based Browsers (Examples: Google Chrome, Microsoft Edge, Opera, Brave, Vivaldi)
- Apple Safari for MacOS and iPadOS.
- Mozilla Firefox.

{{< hint type=important title=Information >}}
A desktop class browser is necessary to administrate and modify your vBulletin Software. Much of the administrator functionality may not work properly on screens smaller than 10 inches (25.4 cm).
{{< /hint >}}

## More Information

This information changes depending the the version. For the most up to date list see this [forum topic](https://forum.vbulletin.com/node/4387853).