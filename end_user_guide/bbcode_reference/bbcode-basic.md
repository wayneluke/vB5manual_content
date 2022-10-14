---
Title: "Basic BBCode"
Slug: basic-bbcode
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 2
Description: Basic BBCode allows the basics of document formatting. The BBCode included here are font, color, size, bold, italic, underline, and alignment.
---

<p>Basic BBCode allows the basics of document formatting. The BBCode included here are font, color, size, bold, italic, underline, and alignment.</p>
<div class="restore">
	<table>
		<tr>
			<th style="text-align:left;" colspan="2">Font</th>
		</tr>
		<tr>
			<td class="definition" colspan="2"><p>This tag allows you to change the font or type style of your text.<br />Available Fonts: <span style="font-family:Arial;">Arial</span>, <span style="font-family:'Comic Sans MS';">Comic Sans MS</span>, <span style="font-family:'Courier New';">Courier New</span>, <span style="font-family:Georgia;">Georgia</span>, <span style="font-family:'Lucida Sans Unicode';">Lucida Sans Unicode</span>, <span style="font-family:'Tahoma';">Tahoma</span>, <span style="font-family:'Times New Roman';">Times New Roman</span>, <span style="font-family:'Trebuchet MS';">Trebuchet MS</span>, <span style="font-family:'Verdana';">Verdana</span>.</p></td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[font=option]value[/font]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[font=Georgia]This text is in the Georgia type style.[/font]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td ><span style="font-family:Georgia;">This text is in the Georgia type style.</span></td>
		</tr>
		<tr>
			<th style="text-align:left;" colspan="2">Bold, Italic and Underline</th>
		</tr>
		<tr>
			<td class="definition" colspan="2">These codes provide basic formatting to your text.</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[b]value[/b]<br />[i]value[/i]<br />[u]value[/u]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[b]This is bold text.[/b]<br />[i]This is italic text[/i]<br />[u]This is underlined text[/u]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td ><b>This is bold text.</b><br /><i>This is italic text</i><br /><span style="text-decoration:underline">This is underlined text.</span></td>
		</tr>
		<tr>
			<th style="text-align:left;"  colspan="2">Color</th>
		</tr>
		<tr>
			<td class="definition" colspan="2">Allows you to color your text. You can use any named color or hex value. Colors can also be selected using the built-in color palette tool.</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[color=option]value[/color]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[color=blue]This text is blue.[/color]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td ><span style="color:blue;">This text is blue.</span></td>
		</tr>
		<tr>
			<th style="text-align:left;" colspan="2">Size</th>
		</tr>
		<tr>
			<td class="definition" colspan="2">Allows you to change the size of your text. Allows font sizes from 8 pixels to 72 pixels in size.</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[size=option]value[/size]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[size=18]This text is 18 pixels tall[/size]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td ><span style="font-size:18px">This text is 18 pixels tall</span></td>
		</tr>
		<tr>
			<th style="text-align:left;" colspan="2">Left / Right / Center Justification</th>
		</tr>
		<tr>
			<td class="definition" colspan="2">Allows you to align or justify your text for different effects.</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[left]value[/left]<br />[center]value[/center]<br />[right]value[/right]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[left]this text is left-aligned[/left]<br />[center]this text is center-aligned[/center]<br />[right]this text is right-aligned[/right]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td ><div align="left">this text is left-aligned</div><div align="center">this text is center-aligned</div><div align="right">this text is right-aligned</div></td>
		</tr>
		<tr>
			<th style="text-align:left;" colspan="2">Indent</th>
		</tr>
		<tr>
			<td class="definition" colspan="2">Allows you to indent your text within a blockquote element.</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[indent]value[/indent]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[indent]This text is indented.[/indent]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td ><blockquote>This text is indented.</blockquote></td>
		</tr>
		<tr>
			<th style="text-align:left;" colspan="2">noparse</th>
		</tr>
		<tr>
			<td colspan="2">Tells the system to not parse BBCODE</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>[noparse][b]option[b][/noparse]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>[noparse][b]Lorem ipsum dolor sit amet[/b][/noparse]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td >[b]Lorem ipsum dolor sit amet[/b]</td>
		</tr>
		<tr>
			<th style="text-align:left;" colspan="2">User Mentions</th>
		</tr>
		<tr>
			<td class="definition" colspan="2">
				Allows you to mention and link another user to the conversation. The mentioned user will get a notification about the mention.
				This BBCode works off the @ nomenclature popular by Twitter and Facebook. However you can use it as a standard BBCODE as well.
				Using the @ format in WYSIWYG mode, will trigger an auto-suggestion dropdown. For names with spaces, use double quotes
				to clarify your meaning.
			</td>
		</tr>
		<tr>
			<td>Usage:</td>
			<td>@%username%<br>[user]value[/user]</td>
		</tr>
		<tr>
			<td>Example Usage:</td>
			<td>@"John Doe"<br>@John Doe<br>[user]John Doe[/user]</td>
		</tr>
		<tr>
			<td>Example Output:</td>
			<td>@<a href="#">John Doe</a><br>@<a href="#">John</a> Doe<br>@<a href="#">John Doe</a><br></td>
		</tr>
	</table>
</div>

<hr>
<small>
updated: 2021-10-06 01:30pm | Version: 5.6.5 Alpha 11
</small>