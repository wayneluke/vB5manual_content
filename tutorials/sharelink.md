---
title: 'Creating a New Share Button'
slug: adding_share_button
weight: 1
---


# Creating a new Share button

If you want to add a new share button within posts, knowing where to start can be intimidating.

## Creating a custom template.

To start the process, you need to create a new template to hold your custom HTML code.

1. In the AdminCP go to Styles → Style Manager.
1. Select your style row and go to the Choose Action drop down. Note: If you are creating a product (see below), you should choose the MASTER STYLE which will be in the list while the site is in Debug Mode.
1. Select "Add New Template" from the drop down.
1. Add your custom code.
1. Give the template a name. Something like "display_linkedin_share" would be appropriate but it can be anything you want.
1. Save this new template.
1. If you use multiple templates, then repeat for each style or create a product to hold the template in the MASTER STYLE (see below)

## Building the hook
In order to show your new template it needs to be tied to a template hook. These are small pieces of code within vBulletin that tells the system to find and include any template at specific locations. For a share button, the hook that you want to use is conversation_share.

1. Go to Products and Hooks → Manage Templates Hooks
1. Click on "Add New Hook"
1. If using a Product (see below) select your product from the drop down.
1. Set the Hook Location to "conversation_sharing"
1. Give it a name like "LinkedIn Share" or whatever you want.
1. Set the template name to the template that you created above.
1. Save the Hook.
1. This should give you a working link in each post. If you want to style it like the others then look at the b-sharing-menu* CSS in the default templates.

## Creating a Product 

> Note: This creating Products is not available on vBulletin Cloud. However, the other portions can be completed on vBulletin Cloud. 
 
Products allow you to apply more permanence to your changes. When you upgrade vBulletin, there is a possibility for your changes to be erased because they are assigned to the vBulletin product by default. During an upgrade, some parts of the system are replaced with new objects. This includes unedited templates, phrases, settings, and permissions. 

Creating your own product provides a wrapper that protects your customizations. A product also allows you to easily apply your changes to every style or language, even ones added in the future. 

1. Put your site into Debug Mode
2. Go to Products & Hooks.
3. Click Add New Product.
4. Give it a Product ID. All lower case, no spaces.
5. Give it a title.
6. The rest is optional.
7. Save your Product.
8. Complete the steps for creating a template and hook above.