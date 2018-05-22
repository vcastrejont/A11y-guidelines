
# DOCUMENT

## Language
Declaring a language attribute on the HTML element enables a screen reader to read out the text with correct pronunciation.

Specify a language with the lang attribute on the html element, example: `<html lang="en">`

**How to test:** Manually test or using wave testing tool.

# LANDMARKS

Landmarks have a very important role in semantics, html has a wide variety of tags that are specific for every part of a website, we recommend to use them correctly for each case.

Roles are part of the html 5 standard now they help screen reader users to identify the part of a website, many html tags have now an intrinsic role that you can take advantage of but If you use the common `<div>` tags for the layout you need to add a role manually, example:

    <div id="mainContent" role="main">

These are the most common landmarks tags currently available:

## Main

The `<main>` tag specifies the main content of a document. This will help screen readers and other assistive technologies understand where the main content begins. Use only once per document.

**How to test:** Manually test or use a testing tool

## Banner

Banners are a convention used on most web sites to convey branding such as the logo, identity and may also be used as a location for advertising information or include the search form, they are placed typically at the top of the website. You can only have one `role=”banner”` per document, example:

	<header role="banner">...</header>
	
**How to test:** Manually test or use a testing tool

# Header

The HTML `<header>` element represents introductory content, typically a group of introductory or navigational aids. You can have several `<header>` elements in one document if they don't have the role banner assigned.

## Nav

The `<nav>` tag represents a section of a page whose purpose is to provide navigation links, either within the current document or to other documents.

Notice that not all links of a document should be inside a `<nav>` element. This element is intended only for major block of navigation links. A document may have several `<nav> `elements.
