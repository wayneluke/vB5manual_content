---
title: Style Variables
slug: style_variables
weight: 4
---

StyleVars (short for Style Variables) are PHP variables that contain a single value used to control the appearance of some aspect of a vBulletin style. Stylevars are used in conjunction with CSS and Templates to control the look and feel of your vBulletin site.

## How Style Variables Interact with CSS 

vBulletin uses Style Variables to dynamically build the CSS it uses for rendering during page load or when the files are written to the server, if you have enabled that option. 

StyleVars are incorporated into CSS and Templates using the {vb:stylevar} syntax. 

While Stylevars are primarily used within CSS in vBulletin, they can be used in HTML templates as well.

Here is a sample of code in a CSS template:

```
.b-userinfo {
	text-align: center;
	color: {vb:stylevar post_user_info_color};
	padding: 15px 15px 10px;
}

.b-userinfo--pmchat {
	display: inline-block;
}

.b-userinfo__rank {
	/* TODO: is this really the stylevar we want to use? */
	color: {vb:stylevar post_controls_text_color};
}

.b-userinfo__icons {
	position: absolute;
	bottom: 10px;
	{vb:stylevar left}: 10px;
}
```

This code contains several style variable references denoted by {vb:stylevar} tags. The vBulletin template engine retrieves the values of the style variables and inserts them directly into the CSS before it is used for rendering.

### CSS Math Tag

It is possible to use style variables in mathematical expressions with the {vb:math} tag.

This is used to evaluate the result of the mathematical expression specified. The syntax is `{vb:math expression}`. 

An example using {vb:math} is:

```
height:{vb:math 8px + {vb:math {vb:stylevar font.fontSize}-1}};
```

This expression determines the height of an element based on the font size specified in the font style variable and an extra value of 8 pixels.