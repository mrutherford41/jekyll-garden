---

layout: new
title: A Day of Learning How to Edit Jekyll Themes
categories: mind
published: false

---

Now that I have succeeded in learning how to add new posts and pages I wanted to see if I could make some style changes.

This included a lot of trial and error to learn how all of the files includes, layouts, assets worked together but once the foundations were laid it all made sense and was easy to customize.

I was satisfied with the default theme and just wanted to see if I could add a background image section right above the page title/content to begin.

**These are the tutorials I found which helped me get started**

[Editing Jekyll Theme CSS](https://mrmarchant.com/editing-jekyll-theme-css-for-github-pages/)

[Overriding Theme Defaults](https://github.com/jekyll/jekyll/blob/1008f1b4e32ed7f82d5d8a0d610b670b2a3b4454/docs/_docs/themes.md#overriding-theme-defaults/)

I wanted to keep the original files untouched as a backup so the new layout will be made up of new files using the original as a foundation.

<br>
<span class="post_headings">Copying Default Layouts to Root Directory</span>

By default the minima theme places all of the style and layout files in a separate folder from the root directory. In order to copy what I needed from these files I had to find them and copy them over to the root.

To find where these files are located:

`bundle info --path minima`

On Windows these files were located in:

![bundle info path](/assets/images/screenshot2.jpg)

Here I copied the includes, layout, and assets folders to my site directory to have as backup. 

The original theme files located above will continue to be used but copying them over to root allows easy access to copy anything we need for our new styles.

Import Minima Theme for a Foundation
{:.post_headings}

The first step was to create a new scss file which goes in a folder called /assets/css.

![import theme screenshot](/assets/images/shot3.jpg)

These allows you to keep the minima theme while adding your own custom styles.

### Create A New Layout

Copy the default.html code and paste it into the new layout post_edit.html

Create a new layout html file which I named post_edit.html.

Copy the code from the default.html layout file and past it into the new file. Here I can change the linked css file to the one I created. 

	<link rel="stylesheet" href="/assets/css/style1.css">

Now any styling I add to this stylesheet will affect the new layout.

### Add the Layout to a Page

Now any page or post I want to have this layout I just add to the frontmatter at the top.

	---

	layout: post_edit

	---


### Make Changes to Style

Now I can add the new section background

	<section class="bg-img"></section>

<br>
<div class="title-underline" markdown="1">
	
### The Final Result

</div>

![final_layout](/assets/images/final_result.png)
