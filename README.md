My News
=====================
2016-11-26


My personal home news feed (sort of).


[![my-news.png](https://s19.postimg.org/uo1n9wiqr/my_news.png)](https://postimg.org/image/i9ev9kr8f/)


What is it for?
---------------

How do you keep an eye on what's interesting to you on the web ? twitter ? a news feed ?

I use the following script:


```html
<!DOCTYPE html>
<html>
<head>
	<title>My News</title>
</head>
<body>


	<ul id="remote">
		<li><a target="_blank" href="https://developers.google.com/web/updates/?hl=en">google developers web updates</a></li>
		<li><a target="_blank" href="https://plus.google.com/+GoogleDevelopers">google plus > google developers</a></li>
		<li><a target="_blank" href="https://customelements.io/">custom elements</a></li>
		<li><a target="_blank" href="https://material.uplabs.com/">uplabs</a></li>
		<li><a target="_blank" href="https://material.google.com/material-design/whats-new.html">material what's new</a></li>
		<li><a target="_blank" href="https://www.polymer-project.org/1.0/docs/release-notes">polymer release notes</a></li>
		<li><a target="_blank" href="https://annevankesteren.nl/2016/">annevankesteren</a></li>
		<li><a target="_blank" href="https://github.com/w3c/webcomponents">web components w3c</a></li>
		<li><a target="_blank" href="https://www.sitepoint.com/">site point</a></li>
		<li><a target="_blank" href="http://alistapart.com/">a list apart</a></li>
		<li><a target="_blank" href="http://searchengineland.com/library/channel/seo">search engine land</a></li>
		<li><a target="_blank" href="https://www.filamentgroup.com/lab/">filament group</a></li>
		<li><a target="_blank" href="https://robdodson.me/">rob dodson</a></li>
		<li><a target="_blank" href="https://infrequently.org/">infrequently</a></li>
		<li><a target="_blank" href="https://plus.google.com/u/0/+FrancoisBeaufort">F. Beaufort</a></li>
		<li><a target="_blank" href="https://github.com/googlecartographer">Cartographer</a></li>
		<li><a target="_blank" href="http://jonrimmer.github.io/are-we-componentized-yet/">are we componentized yet?</a></li>
		<li><a target="_blank" href="https://threatpost.com/">threatpost</a></li>
		<li><a target="_blank" href="https://www.exploit-db.com/">exploitdb</a></li>
		<li><a target="_blank" href="http://www.videocopilot.net/blog/">videocopilot</a></li>
	</ul>

	<script>

		var screen = window.open();



		var remote = document.getElementById('remote');
		remote.addEventListener('click', function(e){
			e.preventDefault();
			var el = e.target;
			if(el.matches("a")){
				screen.location.href = el.href;
			}
		});



	</script>


</body>
</html>
```


And, I've configured my server so that I access it by typing "news" in the url.

So, every time I want to see if things that I have an interest into have evolved, I just type ne...ws in the browser, and an ugly list of my favorite links will be displayed, but wait...

That's not the end of the story.
It will also create a second tab, which is a viewer window.

So what I do after typing news is drag the second tab out to a new window, and then I resize my list of links, and there I have it: my personal news feed.

I can just click on the links on the left and it updates the window on the right.



Might not be the coolest thing, but works fine for me, hope you enjoy.
















