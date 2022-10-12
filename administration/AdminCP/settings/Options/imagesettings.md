---
Title: "Image Settings"
Slug: image-settings
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 03:12pm"
Weight: 70
---


## Image Processing Library

Choose the image processing library that vBulletin will use for processing thumbnails and avatars.  GD is more widely available but ImageMagick is more robust, supporting more image types. ImageMagick must have a valid path chosen below.




- Variable Name: imagetype
- Data Type: free
- Default Value: GD

## ImageMagick Binary Path

Path to the ImageMagick 6 binaries (<i>convert</i> and <i>identify</i>). Example:<br /><br />
Unix: /usr/local/bin/<br />
Windows: C:\imagemagick\
<br /><br />
This option is only used if "Image Processing Library" is set to "ImageMagick 6".




- Variable Name: magickpath
- Data Type: free
- Default Value: 

## Enable PDF Thumbnails

Using the ImageMagick or Imagick processing library, you can enable thumbnails for PDF attachments if GhostScript is installed on your server. 
This option only takes effect if using "ImageMagick 6" or "Imagick (PHP Extension)" for "Image Processing Library" option above.




- Variable Name: imagick_pdf_thumbnail
- Data Type: boolean
- Default Value: 0

## GD Resize Quality

Uploaded images are automatically recreated by the image handler for security purposes. When using the GD image library, a created JPEG file may result in a larger size than the original image. This option controls the trade off between file size and image quality, from 0 (worst quality, smallest size) to 100 (best quality, largest size). <br /><br />

The default is suitable for most sites.




- Variable Name: gdresizequality
- Data Type: integer
- Default Value: 90


<hr>
<small>
updated: 2021-10-06 03:12pm | Version: 5.6.5 Alpha 11
</small>