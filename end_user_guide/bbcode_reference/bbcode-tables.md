---
Title: "Creating Tables"
Slug: creating-tables
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 8
Description: Tables are used to format and control tabular data. Like a spreadsheet. The software supports basic table functionality to allow this.
---

<p>Tables are used to format and control tabular data. Like a spreadsheet. The software supports basic table functionality to allow this.</p>

<div class="restore">
<table>
	<tr>
		<th style="text-align:left;" colspan="2">Table</th>
	</tr>
	<tr>
		<td colspan="2">This is the container tag. It contains multiple rows and multiple cells per row.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[table][tr][td][/td][/tr][/table]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[table]<br />[tr]<br />[td]value[/td]<br />[td]value[/td]<br />[/tr]<br />[/table]</td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Table Row</th>
	</tr>
	<tr>
		<td colspan="2">Rows setup the basis for your indivdiual cells and provide additional structure to the table.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[tr]<br />[td]value[/td]<br />[td]value[/td]<br />[/tr]</td>
	</tr>
		<tr>
		<th style="text-align:left;" colspan="2">Table Cell</th>
	</tr>
	<tr>
		<td colspan="2">Table cells actually hold the content of your table.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[td]value 1[/td]<br />[td]value 2[/td]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td><table border="1"><tr><td>value 1</td><td>value 2</td></tr></table></td>
	</tr>
	<tr>
		<th style="text-align:left;" colspan="2">Combined example output.</th>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td >
		<table>
			<tr>
				<td>Name</td>
				<td>Posts</td>
			</tr>
			<tr>
				<td>John</td>
				<td>1,203</td>
			</tr>
			<tr>
				<td>Sally</td>
				<td>1,902</td>
			</tr>
			<tr>
				<td>Joe</td>
				<td>73</td>
			</tr>
			<tr>
				<td>Tim</td>
				<td>843</td>
			</tr>
			<tr>
				<td>Marcie</td>
				<td>1,076</td>
			</tr>
			<tr>
				<td>Tom</td>
				<td>684</td>
			</tr>
		</table>
		</td>
	</tr>
</table>
</div>

<hr>
<small>
updated: 2021-10-06 01:30pm | Version: 5.6.5 Alpha 11
</small>