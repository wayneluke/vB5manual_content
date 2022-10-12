---
title: Upgrading from Legacy Versions
slug: upgrading_from_legacy_versions
weight: 1
---
## What to know before you upgrade from vB3 or vB4

Upgrading any major software platform should be carefully thought through beforehand; for many of you, vBulletin is the heart of your site. Here are some things to consider when upgrading:

- {{< color "secondary" >}}Some functionality may have been deprecated and not will not be carried forward.{{< /color >}}
- Data structures are completely different. The vBulletin 5 Connect upgrade script will upgrade your existing data to the new format. After this is completed, there is **no way to revert** to an older version.
- Styles from previous versions are not compatible. Any customizations will need to be reapplied. If you use a custom color palette, you should write down the color codes and where each color is used so they can be reapplied.
- Addon Products, Hooks, and most Template modifications from older versions will not be applicable in vBulletin 5 Connect. These will need to be re-coded to work in the current system.

### Empty Directory

If you look at the `upload` directory of your vBulletin Package, you will see that the file structure for vBulletin Connect is different than the file structure for legacy versions. vBulletin 5 needs to be installed in an empty directory without the legacy files present. If you store attachments and/or custom avatars within the file system, you will want to restore these directories after uploading the vBulletin 5 file structure.

### Questions to Ask

1. Have you installed any plugins or products? If so, the first thing that you will need to decide is “Is this critical to my site?”
   - If the answer is yes, you will first need to check that a vB5 compatible version of the modification is available, either at www.vbulletin.org or via the author’s own site.
   - If the answer is no, then you need take no action as vBulletin 5’s new API system means that any existing plugins and products won’t work - however after you upgrade, it would be good practice to make sure you remove any files required by these.
2. vBulletin 5’s template code has been rewritten from scratch so existing themes/styles from vB4 will not work with it. As with plugins and products, if you’re looking to retain a similar look and feel to your site or simply don’t wish to use the default style after upgrading, you will need to do one of three things:
   - Contact the style designer to see if they’ve already created a vB5 compatible version of the style.
   - Download and install a new vB5 compatible style from www.vbulletin.org or another supplier or
   - Create a test installation of vB5 and create your own unique style from scratch
3. Variables used within templates may have changed. This means that any variable reference in vBulletin markup will need to be updated. 
4. Are you running a big board? We know that upgrading a big board can be complicated and has its own set of issues. Please upgrade a test version of your site first. 
5. Do you use a custom .htaccess file on your site? As vBulletin 5 comes with URL Rewrites as standard, it includes an .htaccess by default. Uploading the files for the upgrade will see your custom .htaccess file overwritten losing any custom code that you had within the file (URL Rewrites, specific filetype caching). Make sure you have a backup of your .htaccess file before proceeding with the upgrade then you can look to merge the contents of your custom file and the vBulletin 5 default file after upgrading.

### Frequently Asked Questions
- {{< color "secondary" >}}Can I make my URLs look like vBSEO?{{< /color >}}:  No, this is not possible in vBulletin 5. It comes with its own URL and route structure.
- {{< color "secondary" >}}The person who created my custom style isn't available to upgrade it. Can you do this for me?{{< /color >}}: No, we do not perform customizations. vBulletin 5 Connect comes with a number of themes when it is installed. You can use one of these until you perform your customizations.
- {{< color "secondary" >}}Can I install this software in a test installation?{{< /color >}}: Yes. This is the recoommended process.
