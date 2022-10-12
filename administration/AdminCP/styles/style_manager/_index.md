---
title: Style Manager
slug: style_manager
weight: 1
---

The Style Manager is the facility to use to create and edit vBulletin styles, which control the way your vBulletin installation appears to your visitors. Styles include color and font changes, as well as template changes that alter the layout of the site.

The following is a list and descriptions of the various controls (left to right) on the initial screen of the Style Manager.

- **Title**: Administrators can click to open a new window that shows the public area of your site with this style applied, even if general users are not able to use that particular style. 
- **Active**: Sets whether or not the style is available for non-administrators to use. If the checkbox for a style is cleared, only administrators are able to use that style.
- **Display Order**: The number in the small text box in the middle of the screen specifies the display order of a style. Higher numbers are displayed later in the listing. The number makes no difference to the content of the style and is used solely for display order convenience.
- **Controls**: This selection menu contains links to pages where you can make changes to the style, for example to change the style’s title or download the style as a style.xml file.
  - Edit Templates: This shows the list of templates in this style. All styles inherit their default templates from their parent. Any changes here will be merged into templates released with new versions as long as it is possible.
  - Add New Template: Allows you to add a new custom template to a style. Custom templates are useful if you plan on using template hooks to add custom features.
  - Style Variable Editor: Style Variables are used to control the look of your site. These variables are converted to CSS that tells the browser how to draw your site.
  - Replacement Variables: Replacement Variables allow you create global replacements for any word. This allows you another layer of customization in a site.
  - Add Child Style: Creates a new style based on the values of its parents. Allows you to quickly make multiple variations of a customized style. Child styles  are used for vBulletin Themes so that customers can change the logo and other style variables without worrying about these changes being overwritten on upgrades.
  - Download: Allows you to download the current style in XML format. The XML files can be used for backup purposes or to share the style with others.
- **Templates**: Click this button to open or close the list of templates for the selected style.

{{< hint type=note >}}
When a vBulletin site is in debug mode, additional styles will be shown. These styles will be marked with a red asterisk when using the default AdminCP color theme. Any changes to these styles will be overwritten on upgrades. 
{{< /hint >}}