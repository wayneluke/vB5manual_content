---
Title: "Using Code Snippets"
Slug: using-code-snippets
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 9
Description: Displaying Code within a topic often requires special handling to preserve formatting and prevent it from being parsed by the end-user's client.
---

Displaying Code within a topic often requires special handling to preserve formatting and prevent it from being parsed by the end-user's client.

<div class="restore">
<table>
	<tr>
		<th style="text-align:left;" colspan="2">Code</th>
	</tr>
	<tr>
		<td colspan="2">The [code] tag switches to a fixed-width (monospace) font and preserves all spacing. Note: If you have permission to post HTML, it will be parsed. If you do not wish HTML to be parsed, you should surround it with [noparse] tags.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[code]value[/code]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[code]&lt;script type="text/javascript"&gt;<br />&lt;!--<br />&nbsp;&nbsp;alert("Hello world!");<br />//--&gt;<br />&lt;/script&gt;<br />[/code]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td >
			<div class="bbcode_container">
				<div class="bbcode_description">Code:</div>
				<pre class="bbcode_code" style="height:84px;">
&lt;script type="text/javascript"&gt;
&lt;!--
	alert("Hello world!");
//--&gt;
&lt;/script&gt;
				</pre>
			</div>
		</td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">HTML Code</th>
	</tr>
	<tr>
		<td colspan="2">The [html] tag allows you to perform syntax highlighting for HTML code.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[html]value[/html]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[html]<br />&lt;img src="image.gif" alt="image" /&gt;<br />&lt;a href="testing.html" target="_blank"&gt;Testing&lt;/a&gt;<br />[/html]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td >
			<div class="bbcode_container">
				<div class="bbcode_description">HTML Code:</div>
				<pre class="bbcode_code" style="height:48px;">
<span style="color:#800080">&lt;img src=<span style="color:#0000FF">&quot;image.gif&quot;</span> alt=<span style="color:#0000FF">&quot;image&quot;</span> /&gt;</span>
<span style="color:#008000">&lt;a href=<span style="color:#0000FF">&quot;testing.html&quot;</span> target=<span style="color:#0000FF">&quot;_blank&quot;</span>&gt;</span>Testing<span style="color:#008000">&lt;/a&gt;</span>
				</pre>
			</div>
		</td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">PHP Code</th>
	</tr>
	<tr>
		<td colspan="2">The [php] tag performs the same function as the [code] tag, but also adds syntax highlighting for PHP code. Although it is designed for PHP, it may correctly highlight some other C-like languages.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[php]value[/php]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[php]<br />$myvar = 'Hello World!';<br />for ($i = 0; \$i < 10; \$i++)<br />{<br />&nbsp;&nbsp;&nbsp;&nbsp;echo $myvar . "\n";</br />}<br />[/php]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td >
			<div class="bbcode_container">
				<div class="bbcode_description">PHP Code:</div>
				<div class="bbcode_code"style="height:84px;"><code><code><span style="color: #000000">
					<span style="color: #0000BB">$myvar&nbsp;</span><span style="color: #007700">=&nbsp;</span><span style="color: #DD0000">'Hello&nbsp;World!'</span><span style="color: #007700">;<br />for&nbsp;(</span><span style="color: #0000BB">$i&nbsp;</span><span style="color: #007700">=&nbsp;</span><span style="color: #0000BB">0</span><span style="color: #007700">;&nbsp;\</span><span style="color: #0000BB">$i&nbsp;</span><span style="color: #007700">&lt;&nbsp;</span><span style="color: #0000BB">10</span><span style="color: #007700">;&nbsp;\</span><span style="color: #0000BB">$i</span><span style="color: #007700">++)<br />{<br />&nbsp;&nbsp;&nbsp;&nbsp;echo&nbsp;</span><span style="color: #0000BB">$myvar&nbsp;</span><span style="color: #007700">.&nbsp;</span><span style="color: #DD0000">"\n"</span><span style="color: #007700">;<br />}&nbsp;<br /></span><span style="color: #0000BB"></span></span></code></code>
				</div>
			</div>
		</td>
	</tr>
</table>
</div>

<hr>
<small>
updated: 2021-10-06 01:30pm | Version: 5.6.5 Alpha 11
</small>