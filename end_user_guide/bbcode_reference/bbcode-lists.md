---
Title: "Creating Lists"
Slug: creating-lists
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 7
Description: Lists allow you to create bulleted points for your topic.
---

Lists allow you to create bulleted points for your topic.

<div class="restore">
<table>
	<tr>
		<th style="text-align:left;" colspan="2">Bulleted Lists</th>
	</tr>
	<tr>
		<td colspan="2">The [list] tag allows you to create simple, bulleted lists without specifying an option. Within the value portion, each bullet is denoted by the [*] tag.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[list][*]item,[*]item, ...[/list]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[list]<br />[*]list item 1</br >[*]list item 2</br />[/list]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td ><ul><li>list item 1</li><li>list item 2</li></ul></td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Advanced Lists</th>
	</tr>
	<tr>
		<td colspan="2">The [list] tag allows you to create advanced lists by specifying an option. The option should have a value of 1 (for a numbered list) or A (for an alphabetic with capital letters list) or a (for an alphabetic with lowercase letters list) or I (for a numbered with capital Roman numeral list) or i (for a numbered with small Roman numeral list).</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[list=option][*]item, [*]item, ...[/list]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[list=1]<br />[*]list item 1<br />[*]list item 2<br />[/list]<br /><br />[list=A]<br />[*]list item 1<br />[*]list item 2<br />[/list]<br /><br />[list=a]<br />[*]list item 1<br />[*]list item 2<br />[/list]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td >
<style>
ol.upper-alpha > li {list-style: upper-alpha outside;}
ol.lower-alpha > li {list-style: lower-alpha outside;}
</style>
<ol><li>list item 1</li><li>list item 2</li></ol><ol class="upper-alpha"><li>list item 1</li><li>list item 2</li></ol><ol class="lower-alpha"><li>list item 1</li><li>list item 2</li></ol></td>
	</tr>
</table>
</div>

<hr>
<small>
updated: 2021-10-06 01:30pm | Version: 5.6.5 Alpha 11
</small>