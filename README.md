# youtube-chords-bookmarklet
Open chords for song from YouTube page with one click.

**pure js:**
```
window.open('https://www.ultimate-guitar.com/search.php?search_type=title&value='+$('.title .ytd-video-primary-info-renderer')[0].text.runs[0].text, '_blank');
```

**bookmarklet encoded:**
```
javascript:void function(a){var b=function(a){window.open("https://www.ultimate-guitar.com/search.php?search_type=title&value="+a(".title .ytd-video-primary-info-renderer")[0].text.runs[0].text,"_blank")};if(a&&a.fn&&1.7<=parseFloat(a.fn.jquery))return void load(a);var c=document.createElement("script");c.src="https://ajax.googleapis.com/ajax/libs/jquery/1/jquery.js",c.onload=c.onreadystatechange=function(){var a=this.readyState;a&&"loaded"!==a&&"complete"!==a||b(jQuery.noConflict())},document.getElementsByTagName("head")[0].appendChild(c)}(window.jQuery);
```

converter:
https://chriszarate.github.io/bookmarkleter/