---
Title: "Creating Links"
Slug: creating-links
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 3
Description: These BBCodes allow you to link to web pages and emails both within and outside the the current site. They make it easier to share information.
---

<p>These BBCodes allow you to link to web pages and emails both within and outside the the current site. They make it easy to share information.</p>
<p>Note: Most links to webpages will be converted automatically by the site. However some protocols may still need the link tag.</p>

<div class="restore">
<table>
	<tr>
		<th style="text-align:left;" colspan="2">URL Hyperlinks </th>
	</tr>
	<tr>
		<td colspan="2">Allows you to link to other pages or even other sites. This should not be confused with the Link content type described under Creating Content.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[url]option[/url]<br />[url=option]value[/url]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[url]http://www.example.com[/url]<br />[url=http://www.example.com]Check out this link.[/url]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><a href="http://www.example.com">http://www.example.com</a><br /><a href="http://www.example.com">Check out this link.</a></td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Email</th>
	</tr>
	<tr>
		<td colspan="2">Creates and email link that will open in your mail client.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[email]option[/email]<br />[email=option]value[/email]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[email]address@example.com[/email]<br />[email=address@example.com]John Smith[/email]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><a href="mailto:address@example.com">address@example.com</a><br /><a href="mailto:address@example.com">John Smith</a></td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Node</th>
	</tr>
	<tr>
		<td colspan="2">Allows you to create a link to a pre-existing node on the site. This can be a topic, post, forum, blog, group or other content types.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[node]option[/node]<br />[node=option]value[/node]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[node]3456622[/node]<br />[node=3456622]Important Topic[/node]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><a href="http://example.com/forum/node/3456622">3456622</a><br /><a href="http://example.com/forum/node/3456622">Important Topic</a></td>
	</tr>
</table>
</div>

<hr>
<small>
updated: 2021-10-06 01:30pm | Version: 5.6.5 Alpha 11
</small>