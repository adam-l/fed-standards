# Coding Standards
Below is a set of my personal coding standards, guidelines and best practices that I made for myself and for recommending to others. Those are the results of many years of experience in working on a variety of online projects with a variety of professionals.

If you have any good ideas on how my set of standards might be improved, please don't hesitate to share those with me. I am always open to hear suggestions of this sort.

## Table of Contents
<ul>
	<li><a href="#preliminaries-setting-your-editor">Preliminaries - Setting Your Editor</a>
		<ul>
			<li><a href="#line-endings">Line Endings</a></li>
			<li><a href="#encoding">Encoding</a></li>
			<li><a href="#indentation">Indentation</a></li>
			<li><a href="#plugins">Plugins</a></li>
		</ul>
	</li>
	<li><a href="#html-coding-standards">HTML Coding Standards</a>
		<ul>
			<li><a href="#doctype">Doctype</a></li>
			<li><a href="#">Indendation</a></li>
			<li><a href="#">Conditional comments</a></li>
			<li><a href="#">Single Line Comments</a></li>
			<li><a href="#">Attribute order</a></li>
			<li><a href="#">Most overused HTML tags</a></li>
		</ul>
	</li>
	<li><a href="#css">CSS Coding Standards</a>
		<ul>
			<li><a href="#">Multiline syntax</a></li>
			<li><a href="#">Selectors</a></li>
			<li><a href="#">!important rule</a></li>
			<li><a href="#">Shorthands</a></li>
			<li><a href="#">Minification</a></li>
			<li><a href="#">Sprites</a></li>
			<li><a href="#">Property order</a></li>
			<li><a href="#">Fallback backgrounds</a></li>
		</ul>
	</li>
	<li><a href="#js">JS Coding Standards</a>
		<ul>
			<li><a href="#">Quotation Marks</a></li>
			<li><a href="#">Whitespace</a></li>
			<li><a href="#">CamelCase</a></li>
			<li><a href="#">Constructors</a></li>
			<li><a href="#">Namespace</a></li>
		</ul>
	</li>
	<li><a href="#workflow">FED Workflow</a>
		<ul>
			<li><a href="#">Creating common elements</a></li>
			<li><a href="#">Assuring quality - the checklist</a></li>
		</ul>
	</li>
</ul>

***

#Preliminaries - Setting Your Editor
## Line Endings
Choose one type of line endings for the project that you and the rest of the team is working on. UNIX line endings are the most common ones and they are generally recommended for avoiding problems that might arise when the document migrates between users and operating systems.

### Resources:
* <a target="_blank" href="http://docs.sublimetext.info/en/latest/reference/settings.html#system-and-miscellaneous-settings">Sublime Text Docs: System and Miscellaneous Settings</a>

***

## Encoding
UTF-8 encoding dominated the Wold Wide Web and is generally the most recommended option when it come's to encoding. UTF-8 can for example prevent you from issues common for data migration.

### Resources:
* <a target="_blank" href="http://googleblog.blogspot.com/2010/01/unicode-nearing-50-of-web.html">Google Official Blog: Unicode nearing 50% of the web</a>
* <a target="_blank" href="http://www.utf8everywhere.org/">UTF-8 Everywhere</a>
* <a target="_blank" href="http://annevankesteren.nl/2009/09/utf-8-reasons">Technical Reasons To Use UTF-8</a>

***

## Indentation
I prefer using tabs over spaces. I use one tab character for indentation. I believe that a good developer should adapt to the way the team decided to work (whenever it's reasonable). That means that even when you prefer to use tabs - just like myself - you should switch to spaces if this the way your team is already working.

### Resources:
* <a target="_blank" href="http://chimera.labs.oreilly.com/books/1234000001640/ch01.html#you_sho">Nicholas Zakas - Maintainable JavaScript (video transcript)</a>

***

## Plugins
I do not use many plugins when I write code. One plugin that I personally find very useful and can recommend is <a target="_blank" href="http://docs.emmet.io/">Emmet</a> (ex-Zen Coding).

### Resources:
* <a target="_blank" href="http://coding.smashingmagazine.com/2013/03/26/goodbye-zen-coding-hello-emmet/">Goodbye, Zen Coding. Hello, Emmet!</a>

***

# HTML Coding Standards
## Doctype
Enforce standards mode in web browser by putting a doctype at the beginning of your HTML document. Having the doctype is also neccessary for validating against HTML and XHTML specifications.

__HTML 4.01 Doctype__
<div class="highlight">
	<pre>&lt;DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"&gt;</pre>
</div>

__XHTML 1.0 Doctype__
<div class="highlight">
	<pre>&lt;!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN" "http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd"&gt;
&lt;html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"&gt;</pre>
</div>

__HTML5 Doctype__
<div class="highlight">
	<pre>&lt;!DOCTYPE html&gt;</pre>
</div>

***

## Indentation
Use proper indentation to maximize code readability.

__Correct__
<div class="highlight">
	<pre>&lt;DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"&gt;</pre>
</div>

__Wrong__
<div class="highlight">
	<pre>&lt;DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd"&gt;</pre>
</div>