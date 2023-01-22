---
title: Knowledge of HTML, CSS and JS
layout: normal
keywords: "websites, building, jekyll, wordpress, brisbane"
description: "Website building services with more than 20 years experience based in Brisbane, Australia"

---
<div class="container justify-content-center">
<div class="row">
<div class="col-12 mb-1">
<p> Remember I said I'd assume you're a beginner? <br/>
<span class="bg-light">HTML = Hypertext Markup Language</span> - It's the text that web pages are written in. Web pages are all written in HTML, whether it's generated or typed manually. This means that you can (in theory) read and understand someone else's code. <br/>
An example of HTML is <code class="bg-light">&lt;p&gt; Hello world&lt;/p&gt;</code> where the angled brackets enclode a 'tag', and in this case the tag is p (paragraph). You must indicate where the paragraph ends with the forward slash (/). Some tags don't need to be ended, such as images. An image is placed with, for example, <code class="bg-light">&lt;img alt="this is an image" src="path-to-the-image"&gt;</code>. There is often a closing tag just before the closing angled bracket.<br/>
I learned HTML by looking at other peoples' code and urge you to do the same. <br/>
A really useful hint is that if you're using Chrome or Firefox (download and develop using both of these. Together they're easily the most used web browsers in the world) you can right-click on a part of a page and select inspect from the context menu. This will open a new pane displaying formatted HTML code, Hover over bits of code and the page will be highlighted, showing you what part of the page that code applies to. You can even double-click to edit parts of the code, if you want to see what the page would look like, even other people's sites.
<br/>There are many places that will take you through tutorials and plenty of reference sites. <a target="_new" href="https://www.w3schools.com/">W3schools is a really good place to start</a>, they also cover CSS and JS</p>
<p><span class="bg-light">CSS = Cascading Style Sheets</span> - These are lines of code intended to change the look of a page or component. You can apply these styles directly to an HTML component. Using the example above, you can apply a style directly to a tag like this: &lt;p style="font-weight:bold;color:red;"&gt;Hello world&lt;/p&gt;, which looks like this when displayed: <span style="font-weight:bold;color:red;">Hello World</span>. That's a style, but not really a style sheet, because it's being applied directly to a tag. The word <em>cascading</em> in CSS refers to the priority system. There are three ways to apply a style, the most normal being to attach an external file containing all of your CSS code, by adding it in your HTML file's head section, for example: <code class="bg-white">&lt;link rel="stylesheet" href="/css/styles.css" type="text/css"&gt;</code>. This tells the web browser that there is a CSS file called <em>styles.css</em> located in a folder called <em>css</em> that is sitting in the root of the web server.<br/>
The second most common way to style your page is to add styles to the head of the page. Instead of the link, you could declare a style code area like this: &lt;style&gt;, put in some style code, e.g.<br/>
&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;p&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;{ font-weight: bold;<br/>&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;color:red;}<br/>This does the same thing to our example paragraph, but you only need to write it once and every paragraph on the page will be red and bold. If you link all of your site's pages to the centralised CSS file in the head, styles.css will affect the whole site.</p>
<p>CSS was developed logically so that the linked file has lowest priority by default, tag specific styling has greatest priority.</p>
<p>In summary:
<ul>
<li> Link a central CSS file to every page </li>
<li> Put page-specific code in the head of the page it will affect </li>
<li> Put tag-specific code in the tag </li>
<li> Tag specific CSS code will override page-specific CSS code, and page-specific CSS code will override a linked file's code </li>
</ul>
</p>
<p>If you want to apply a style to just a part of a paragraph, use &lt;span&gt;. Spans are just to grab part of a sentence and apply a style to it. You will also see a lot of &lt;div&gt; tags. These will start a new line.</p>
<p><span class="bg-light">JS = Java Script</span> - This allows you more flexibility. With javascript you can change CSS classes depending on what the user of your page is doing. I'm not going to cover JS because it gets quite complex but there is an excellent primer at <a target="_new" href="https://developer.mozilla.org/en-US/docs/Web/JavaScript/A_re-introduction_to_JavaScript">Mozilla's developer docs</a>.  </p>
</div><!-- end col -->
</div><!-- end row -->
</div><!-- end container -->
