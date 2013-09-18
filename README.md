# Coding Standards
Below is a set of my personal coding standards, guidelines and best practices that I made for myself and for recommending to others. Those are the results of many years of experience in working on a variety of online projects with a variety of professionals.

If you have any good ideas on how my set of standards might be improved, please don't hesitate to share those with me. I am always open to hear suggestions of this sort.

## Table of Contents
<ul>
	<li><a href="#preliminaries---setting-your-editor">Preliminaries - Setting Your Editor</a>
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
			<li><a href="#indentation-1">Indendation</a></li>
			<li><a href="#">Double quotes for attributes</a></li>
			<li><a href="#lowercase-names">Lowercase names</a></li>
			<li><a href="#">Single line comments</a></li>
			<li><a href="#">Conditional comments</a></li>
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
			<li>
				<a href="#">Reviewing the graphic files - most common problems</a>
				<ul>
					<li>Lack of consitency in the design</li>
				</ul>
			</li>
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
```html
<DOCTYPE HTML PUBLIC "-//W3C//DTD HTML 4.01//EN" "http://www.w3.org/TR/html4/strict.dtd">
```

__XHTML 1.0 Doctype__
```html
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 1.0 Strict//EN"
"http://www.w3.org/TR/xhtml1/DTD/xhtml1-strict.dtd">
<html xmlns="http://www.w3.org/1999/xhtml" xml:lang="en" lang="en"></html>
```

__HTML5 Doctype__
```html
<!DOCTYPE html>
```


***


## Indentation

Use consistent indentation to enhance code readability. I use one tab for each nested element. Your HTML code wil be propably readed several times - i.e. when the CSS based on your mark-up will be created or the back-end developers will work with it.

__Correct__
```html
<article>
	<header>
		<h1>Title</h1>
		<p>Excepteur sint occaecat cupidatat non proident</p>
	</header>
	<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
	<p>Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
	<ul>
		<li>Ut enim ad minim veniam</li>
		<li>Duis aute irure dolor in reprehenderit</li>
		<li>Excepteur sint occaecat cupidatat non proident</li>
	</ul>
	<hr>
	<p>Excepteur sint occaecat cupidatat non proident.</p>
</article>
```

__Wrong__
```html
<article>
<header>
<h1>Title</h1>
<p>Excepteur sint occaecat cupidatat non proident</p>
</header>
<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit.</p>
<p>Ut enim ad minim veniam, quis nostrud exercitation ullamco.</p>
<ul>
<li>Ut enim ad minim veniam</li>
<li>Duis aute irure dolor in reprehenderit</li>
<li>Excepteur sint occaecat cupidatat non proident</li>
</ul><hr>
<p>Excepteur sint occaecat cupidatat non proident.</p>
</article>
```


***


** Double quotes for attributes
I prefer using double quotes for attributes in HTML. By all means however this is not a 'rule of thumb'. It's just my own preference.

What I do think is important however, is that you should be consistent in your choosemenet. Lack of consistency in this case may result in less readable, more confusing code.

__Correct__
```html
<p>
	<label for="email">E-mail address:</label>
	<input id="name" name="email" type="text" />
</p>
```

__Wrong__
```html
<p>
	<label for='email'>E-mail address:</label>
	<input id="name" name='email' type="text" />
</p>
```


***


## Lowercase names 

When you use lowercase and uppercase sings in your HTML it can decrease the readability of your code. It may also cause other problems since XHTML is case sensitive. As uppercase notation would look rather unfamiliar and strange it is a good idea to use lowercase notation for elements, attributes and values.

__Correct__
```html
<input name="SURNAME" TYPE="text" />
```

__Wrong__
```html
<INPUT name="SURNAME" TYPE="text" />
```


***


## Single line comments
I believe that the code that I create should be as much as self-explanatory as possible. I am aware however that in reality this can be sometimes hard to achieve. A good idea is to use an ending comment after a container

__Example__
```html
<div class="sidebar">
	<ul class="nav">
		<li><a href="#">Home</a></li>
		<li><a href="#">Articles</a></li>
		<li><a href="#">About</a></li>
		<li><a href="#">Contact</a></li>
	</ul>
	<!-- / navigation -->

	<div class="author">
		<h2>About author</h2>
		<p>Lorem ipsum dolor sit amet, consectetur adipisicing elit, sed do eiusmod
		tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam,
		quis nostrud exercitation ullamco laboris nisi ut aliquip.</p>
	</div>
	<!-- / about author -->

</div>
<!-- / sidebar -->
```