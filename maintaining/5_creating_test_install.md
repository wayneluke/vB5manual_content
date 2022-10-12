---
title: Creating a Test Installation
slug: creating-test-installation
date: '2021-09-07T20:48:18.034Z'
weight: 5
---

Creating a Test/Development Installation 
When a new version of vBulletin comes out, there's always a clamour for people to be one of the first up and running with the latest version. While in the case of bug fixes, the need to upgrade quickly is understandable, too often people don’t consider what effect an upgrade will have on their site. The following is aimed at providing enough knowledge to be able to create a test 'mirror' of a site so that a test of an upgrade (or any change for that matter!) can be made.

## Step 1 - Update URLs and Backup your database!

An all important step in any upgrade but without it, you'll never be able to test an upgrade - period! As you're going to be moving your database to be read by software on a different URL, you need to make sure you update the database to reflect this. There are two ways to do this:

1. Update the URLs before backing up the database or
2. Update manually in the database after backing up (NOT RECOMMENDED)

To update the URLs before backing up, follow these simple steps:

    Close your site via AdminCP > Settings > Options > Turn Your vBulletin On and Off
    Update the URLs at AdminCP > Settings > Options > Site Name / URL / Contact Details
    Warning:
    ***DO NOT CLOSE YOUR BROWSER AFTER THE ABOVE STEP***
    Backup your database (see below)
    Update the URLs at AdminCP > Settings > Options > Site Name / URL / Contact Details back to your live URLs
    Reopen your site via AdminCP > Settings > Options > Turn Your vBulletin On and Off

This will give you a ready made backup that will require no manual intervention to ensure that it's ready for testing against.

There are a number of ways to backup your database. The most reliable method of backing up and restoring a database is with shell access via ssh. This is because backing up with a PHP script like phpMyAdmin can result in PHP timeouts errors and an incomplete backup file. For more information on how to do this, please see the instructions here:

Backup:
http://www.vbulletin.com/docs/html/maintenance_ssh_backup

If you don't have shell access, some people have also reported success with these scripts:

MySQLDumper:
http://www.mysqldumper.de/en/index.php

MySQLHotcopy:
http://www.vbulletin.com/forum/showthread.php?t=134821&highlight=mysqlhotcopy

Bigdump:
http://www.ozerov.de/bigdump.php

Once you have your backup, you need to actually restore it to be able to test against it.

## Step 2 - Restore your database


There's two options here depending on the hosting package you have:

    Create a new database and restore to it or
    Restore into your live database

Option 1, if you have more than 1 database available to you, is the option we'd recommend in every case because quite simply, it's the safest! That said, some hosting plans, particularly lower costed shared plans, may only allow a user 1 database so you may have no choice but to go with option 2!

Option 1 - Create a new database and restore to it

This is the safest way to go. From your server's control panel, create a new database then restore your freshly backed up database into this new database. As this is a completely separate database to your live one (different database name and hopefully different login details), there will be no need to manipulate the database prior to using it.

Option 2 - Restore into your live database

While this is NOT recommended, there are a number of users who will simply have to go down this route due to the lack of features with the hosting package they have (or can afford). Before doing this, make sure you read these steps BEFORE attempting to do the restore.

To do these, you will need to have a text editor installed. Windows users will have Notepad and Wordpad, Mac users may have TextEdit. I've used Wordpad without issue - and it's Find and Replace tool will be needed for the following steps as you will need these to manipulate the database backup before restoring it but don't worry - it's not complicated as you'll see...

a. Table prefixes

Whether you have prefixes or not, you are going to need to create a prefix to distinguish your test database from your live one. The following shows a table with no prefix then one with a prefix of 'vb_' - the rest of this entry will assume that prefix is currently used:

No Prefix:

DROP TABLE IF EXISTS `access`;
CREATE TABLE `access` (
`userid` int(10) unsigned NOT NULL default '0',
`forumid` smallint(5) unsigned NOT NULL default '0',
`accessmask` smallint(5) unsigned NOT NULL default '0',
PRIMARY KEY (`userid`,`forumid`)
) ENGINE=MyISAM DEFAULT CHARSET=latin1;

With Prefix:

DROP TABLE IF EXISTS `vb_access`;
CREATE TABLE `vb_access` (
`userid` int(10) unsigned NOT NULL default '0',
`forumid` smallint(5) unsigned NOT NULL default '0',
`accessmask` smallint(5) unsigned NOT NULL default '0',
PRIMARY KEY (`userid`,`forumid`)
) ENGINE=MyISAM DEFAULT CHARSET=latin1;

To ensure your test database is unique, you're going to need to add/change the prefix depending on what you currently have in place. Using the 'Find and Replace' option in your editor, you can add/change the prefix very easily (note if you have no prefix you will need to do this twice - once to edit the 'Drop' command, once for the 'Create' one):

Once, you hit OK/Replace All or whatever command your editor has, this will go through and add/replace prefixes on all tables. Now save this file under a different name on your local machine.

Now that you have your edited database, upload this to your server then restore it. For more instructions on using ssh, see this section of the manual:

http://www.vbulletin.com/docs/html/maintenance_ssh_restore

This will create a new set of duplicate database tables within their own 'group' thanks to the amended prefix.

## Step 3 - Files

So, you've got your database in place so all we need is to upload the files - right? Nearly! Yes, you will need to have an actual installation of vBulletin on your server to use these but it's not just a case of uploading the files and away you go - so read on and follow...

First thing's first, create a new empty directory on your server called 'testvb'. You will need to protect this directory from the general public. The most common way to do this is by a combination of .htaccess and .htpasswd files. For more on these and assistance in setting these up, go to:

http://www.htaccesstools.com/htpasswd-generator/

Some Windows Server users may find that this doesn't work for them in which case you should use the permissions tools available on the server

Next, you need to decide what you're doing. Are you testing some changes to the templates etc. without upgrading or are you testing an upgrade?

1. Testing changes

If you're only testing some changes you want to make to the site (new styles, template changes) then either copy your live site's files to the 'testvb' directory or download a copy of your live site and then upload them into the 'testvb' directory.

2. Testing an upgrade

If you're testing an upgrade, then there's no need to copy your live site's files as you're only going to be overwriting them with the newer ones anyway! In this instance, simply download the new files from the Members Area and upload these to your 'testvb' directory.

3. config.php

VERY IMPORTANT STEP! I highlight this as without this step, you'll be doing whatever you do to your live database!

Open config.php in your normal web editor. Again, this will vary slightly depending on whether you're using a different database or whether you're having to use different prefixed tables in the same one.

a. Imported Database to a new database

If you've got the luxury of using a completely separate database, then you will need to edit the following details to ensure you're pointing to the correct one:

    Database Name
    Database Username
    Database Password
    Cookie Prefix

b. Imported Database to different prefixed tables in live database

This is even more important in this scenario. You need to edit the following areas:

    Database Table Prefix
    Cookie Prefix

Why edit the cookie prefix? If you're using the same Cookie prefix on your test site as you do on your live site, your browser won't distinguish which site you're actually viewing as they're both on the same domain. This will cause problems when logging in and doing anything where your personal settings are saved in a Cookie. The easiest way to distinguish these is to change the test site's value to 'vbtest'.

Regardless of which method of database import you've had to do, you should add the following to the top of the config.php file, right under <?php:

define('DISABLE_MAIL', 1);

This will stop the vBulletin email system from sending mails to users on their birthdays, if you add a test post to a subscribed thread etc. The last thing you want is users emailing you to say they've had a notification from a strange URL that looks like it could be your site...

## Step 4 - AdminCP

Almost there! There are a couple of small changes that you will need to make to ensure that things run smoothly! Firstly, we need to make sure all links point to the right directory. So, login to the AdminCP in your testing directory and go to:

Settings → Options → Site URL & Routing


and make sure the Forum URL is pointing to your 'testvb' directory. Also, under the following section, ensure that the 'Path to Save Cookies' setting is set to /testvb/:

Settings → Options → Cookies and HTTP Header Options

And finally, you can also (optionally!) turn off Scheduled Tasks but given that you've disabled the mail system via the config.php file, it would provide benefit to leave this enabled. 