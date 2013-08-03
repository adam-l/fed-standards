# Coding Standards
1Below is a set of my personal coding standards, guidelines and best practices that I made for myself and for recommending to others. These are the result of many years of experience in working on a variety of online projects with a variety of professionals.

If you have any good idea's on how my set of standards might be improved, please don't hesitate to share those with me. I am always open to hear suggestions of this sort.

## Table of Contents
<ul>
	<li><a href="#preliminaries">Preliminaries - Setting Your Editor</a>
		<ul>
			<li><a href="#line-endings">Line Endings</a></li>
			<li><a href="#encoding">Encoding</a></li>
			<li><a href="#indentation">Tabs</a></li>
		</ul>
	</li>
	<li><a href="#html">HTML Coding Standards</a>
		<ul>
			<li><a href="#">Doctype</a></li>
			<li><a href="#">Indendation</a></li>
			<li><a href="#">Conditional comments</a></li>
			<li><a href="#">Single Line Comments</a></li>
			<li><a href="#">Attribute order</a></li>
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
</ul>

<hr>

#Preliminaries - Setting Your Editor
### Line Endings
Choose one type of line endings for the project you and the rest of the team is working on. UNIX line endings are most common type and generally recommended for avoiding problems that might arise when the document migrates between users, and operating systems.

<hr>

### Encoding
UTF-8 encoding dominated the Wold Wide Web and is generally the most recommended option when it come's to encoding. UTF-8 can for example prevent you from issues common for data migration.

#### Resources:
<ol>
	<li><a target="_blank" href="http://googleblog.blogspot.com/2010/01/unicode-nearing-50-of-web.html">Google Official Blog: Unicode nearing 50% of the web</a></li>
	<li><a target="_blank" href="http://www.utf8everywhere.org/">UTF-8 Everywhere</a></li>
	<li><a target="_blank" href="http://annevankesteren.nl/2009/09/utf-8-reasons">Technical Reasons To Use UTF-8</a></li>
</ol>

<hr>

## Tabs
I do not use spaces to for indentation in HTML. I use 1 tab instead and recommend that to others as a general rule.

<hr>

## HTML Coding Standards
### Doctype
Enforce standards mode in web browser by putting a doctype at the beginning of your HTML document. A doctype is also neccessary for validating against HTML and XHTML specifications.

#### HTML5 Doctype
<div class="highlight">
<pre>
<span class="cp">&lt;!DOCTYPE html&gt;</span></pre>
		</div>
		<h3>Indendation</h3>
		<h3>Single line comments</h3>
		<h3>Attribute order</h3>