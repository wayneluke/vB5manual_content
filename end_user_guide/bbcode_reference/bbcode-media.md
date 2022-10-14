---
Title: "Inline Media (Photos and Videos)"
Slug: inline-media-photos-and-videos
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 5
Description: Media allows your content to come alive. vBulletin allows you to embed media including images and videos within your content. These BB Codes explain how to do this manually.
---

Media allows your content to come alive. vBulletin allows you to embed media including images and videos within your content. These BB Codes explain how to do this manually.

<div class="restore">
<table>
	<tr>
		<th style="text-align:left;" colspan="2">Images</th>
	</tr>
	<tr>
		<td colspan="2">The [img] tag allows you to embed images within your posts. You can also combine this tag with the [url] tag to make images become links.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[img]value[/img]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[img]http://www.example.com/images/misc/vbulletin5_logo.png[/img] (Not linked)<br />[url=http://www.example.com] [img]http://www.example.com/images/misc/vbulletin5_logo.png[/img][/url] (Linked)</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><img src="images/misc/vbulletin5_logo.png" /> (Not linked)<br /> <a href="http://www.example.com"><img src="images/misc/vbulletin5_logo.png" /></a></td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Video</th>
	</tr>
	<tr>
		<td colspan="2">The [video] tag allows you to embed videos from various video services within your posts. The best option to insert videos is to use the Link content type or to use the insert video on the Advanced Editor Toolbar. You will have access to more options.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[video]value[/video]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[video=youtube;QTMYrpKDcp8]http://www.youtube.com/watch?v=QTMYrpKDcp8[/video]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><iframe class="restrain" title="YouTube video player" width="640" height="390" src="//www.youtube.com/embed/QTMYrpKDcp8" frameborder="0"></iframe></td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Attachments</th>
	</tr>
	<tr>
		<td colspan="2">The [attach] tag allows you to display an attachment in your post rather than at the bottom. It will only display attachments that belong to the post in which it is utilized. This tag is rarely used directly and included here for completeness.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[attach]attachmentid[/attach]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[attach]12345.txt[/attach]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><p>Output can vary with this. It can display a thumbnail, full sized image or a link to a file. Double clicking on image attachments in the editor will allow you to change their properties. A text link would look like: <br /><a href="12345.txt">12345.txt</a></td>
	</tr>


</table>
</div>

<hr>
<small>
updated: 2021-10-06 01:30pm | Version: 5.6.5 Alpha 11
</small>