---
title: Upgrading vBulletin
weight: 2
slug: upgrading-vbulletin
---

## Preparing the vBulletin Files for Upload 

After you have successfully downloaded the vBulletin package to your computer you will need to prepare the scripts to be uploaded to your web server. We’ve included the instructions for both Windows and MacOS below.

The first thing to do is to decompress the package into its constituent files. If you’ve downloaded the .zip package and your computer is running a recent operating system, you should have all the tools you need to do this.

{{< tabs tabTotal="3" tabID="1" tabName1="Windows" tabName2="MacOS" tabName3="Linux" >}}

{{< tab tabNum="1" >}}

To extract the files from the package, open the folder on your computer where you saved the vBulletin package and right-click on its icon. Choose Extract All... from the pop-up menu.


This will open a wizard to guide you through the unzipping progress. Accept the default options and the system will decompress the files from the zip package.
{{< /tab >}}

{{< tab tabNum="2" >}}

To extract the files from the package, open the folder on your computer where you saved the vBulletin package and right-click (or control-click) on its icon. Choose Open from the pop-up menu.

This will extract all of the files from the package to the current folder.
{{< /tab >}}

{{< tab tabNum="3" >}}

You can unzip the download package with the following command.

`unzip vb5_connect_%version%_%licenseid%.zip`

If you do not have unzip available, you will need to install it via the system's package manager.

{{< /tab >}}
{{< /tabs >}}

###  After Decompressing the Files

When the unzipping progress is complete, you will find that the process has created two new directories. One is called upload and the other is called do_not_upload.

#### upload Directory 

The upload folder contains the vBulletin files that need to be uploaded to your web server.

![upload folder](upload.png)

Rename the upload folder to match the name you gave to the directory containing your vBulletin files on your web server. In this example, the folder containing the vBulletin files is called `forums`.

Note:
If you installed vB5 directly in the root directory of your web publishing folder (not in a subfolder), you do not need to rename the upload folder. Instead, you would upload the contents within this folder to your server.

#### do_not_upload Directory

The do_not_upload folder contains a variety of scripts for advanced management of your site. Unless otherwise specified, they are not necessary for the day to day operations of your site. These files should not be stored on your server. Doing so may create security risks.

![do_not_upload directory](do_not_upload.png)
