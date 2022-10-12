---
Title: "Attachment Options"
Slug: attachment-options
Version: "5.7.0 Alpha 4"
Date: "2022-08-29 09:50am"
Weight: 350
---


## Image Processing Library

Choose the image processing library that vBulletin will use for processing thumbnails and avatars.  GD is more widely available but ImageMagick (Imagick) is more robust, supporting more image types. Imagick requires that both Imagick PHP extension and ImageMagick binaries are installed on the server.




- Variable Name: imagetype
- Data Type: free
- Default Value: GD

## Enable PDF Thumbnails

Using the ImageMagick or Imagick processing library, you can enable thumbnails for PDF attachments if GhostScript is installed on your server. 
This option only takes effect if using "Imagick (PHP Extension)" for "Image Processing Library" option above.




- Variable Name: imagick_pdf_thumbnail
- Data Type: boolean
- Default Value: 0

## GD Resize Quality

Uploaded images are automatically recreated by the image handler for security purposes. When using the GD image library, a created JPEG file may result in a larger size than the original image. This option controls the trade off between file size and image quality, from 0 (worst quality, smallest size) to 100 (best quality, largest size). <br /><br />

The default is suitable for most sites.




- Variable Name: gdresizequality
- Data Type: integer
- Default Value: 90

## Thumbnail Quality

Quality of JPG thumbnails. 75 is a good balance between file-size and image quality.




- Variable Name: thumbquality
- Data Type: integer
- Default Value: 75

## Limit Space Taken Up By Attachments (Total)

Use this option to limit the total combined amount of disk space in bytes that <i>all</i> attachments can occupy.<br />
<br />
Set the option to 0 to have no disk space limit.




- Variable Name: attachtotalspace
- Data Type: number
- Default Value: 0

## Number of thumbnails to show for photo posts

The number of thumbnails shown before opening the lightbox on photo posts (minimum value = 1, maximum value = 15)




- Variable Name: attatchgallerythumbs
- Data Type: integer
- Default Value: 3

## Resize Images

If an image is larger than your maximum allowed dimensions or file-size, an attempt to resize it will be tried.  This may fail if the image is too large to be successfully processed or if the image type is not supported for resizing. When this option is enabled, you should limit the Attachment Input options above to one, otherwise the uploading of multiple large images by one user could strain your server.




- Variable Name: attachresize
- Data Type: number
- Default Value: 1

## View Attached Images Inline

Only affects the "Attached Files" box.<br /><br />
If thumbnails are enabled, thumbnail creation will need to be enabled in the next option.<br /><br />Set this to 'No' if you want to preserve bandwidth or server processor resources.




- Variable Name: viewattachedimages
- Data Type: number
- Default Value: 1

## Advanced Insert Image Popup - Enable

Enabling this option will turn on the Advanced Insert Image Dialog, which will allow users to insert images from the computer, or retrieve images referenced from a URL and store them locally. Disabling this option will display the legacy from URL attachment dialog.




- Variable Name: advimagepopup_enable
- Data Type: boolean
- Default Value: 1

## Attachment Resize Options

Several image sizes are created on demand for uploaded images.  The max dimensions for each size are defined here. Defining a size as "0" will result in that type returning the full size image.




- Variable Name: attachresizes
- Data Type: free
- Default Value: a:5:{s:4:&quot;icon&quot;;i:32;s:5:&quot;thumb&quot;;i:121;s:5:&quot;small&quot;;i:204;s:6:&quot;medium&quot;;i:330;s:5:&quot;large&quot;;i:0;}

## Track Attachment Views

If enabled, this tracks attachment downloads.




- Variable Name: attachmentviewstrack
- Data Type: boolean
- Default Value: 1


<hr>
<small>
updated: 2022-08-29 09:50am | Version: 5.7.0 Alpha 4
</small>