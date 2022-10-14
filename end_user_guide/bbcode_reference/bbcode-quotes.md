---
Title: "Using Quotes"
Slug: using-quotes
Version: "5.6.5 Alpha 11"
Date: "2021-10-06 01:30pm"
Weight: 4
Description: Quotes are a great way to maintain continuity in long conversations. They can be used to provide context and reference posts for replies to posts made hours or days earlier.
---

Quotes are a great way to maintain continuity in long conversations. They can be used to provide context and reference posts for replies to posts made hours or days earlier.

<div class="restore">
<table width="100%">
	<tr>
		<th style="text-align:left;" colspan="2">Quote</th>
	</tr>
	<tr>
		<td colspan="2">The [quote] tag allows you to attribute text to someone else.</td>
	</tr>
	<tr>
		<td>Usage:</td>
		<td>[quote]Quote[/quote]<br />[quote=User Name]value[/quote]<br />[quote=User Name,Node]value[/quote]</td>
	</tr>
	<tr>
		<td>Example Usage:</td>
		<td>[quote]Lorem ipsum dolor sit amet[/quote]<br />[quote=John Doe]Lorem ipsum dolor sit amet[/quote]<br />[quote=John Doe;1]Lorem ipsum dolor sit amet[/quote]</td>
	</tr>
	<tr>
		<td>Example Output:</td>
		<td >
			<div class="bbcode_container">
				<div class="bbcode_quote">
					<div class="quote_container">
						<div class="bbcode_quote_container b-icon b-icon__ldquo-l--gray"></div>
						<div class="message">Lorem ipsum dolor sit amet</div>
					</div>
				</div>
			</div>
			<div class="bbcode_container">
				<div class="bbcode_quote">
					<div class="quote_container">
						<div class="bbcode_quote_container b-icon b-icon__ldquo-l--gray"></div>
						<div class="bbcode_postedby">
							Originally posted by <strong>John Doe</strong>
						</div>
						<div class="message">Lorem ipsum dolor sit amet</div>
					</div>
				</div>
			</div>
			<div class="bbcode_container">
				<div class="bbcode_quote">
					<div class="quote_container">
						<div class="bbcode_quote_container b-icon b-icon__ldquo-l--gray"></div>
						<div class="bbcode_postedby">
							Originally posted by <strong>John Doe</strong>
							<a href="http://www.example.com/forum/main-category/main-forum/15-test-thread?p=16#post16" rel="nofollow" title="View Post" class="b-icon b-icon__double-arrow-right--blue animate-scroll">View Post</a>
						</div>
						<div class="message">Lorem ipsum dolor sit amet</div>
					</div>
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