puzzlescript-embed - Easily embed a PuzzleScript game
=====================================================

puzzlescript-embed allows you to embed a PuzzleScript game into a webpage with only a few lines of HTML and JavaScript.


API
---

```javascript
PuzzleScript.embed(element, id, config)
```

Parameters:

* `element`: parent element for the game canvas. Any child elements will be removed.
* `id`: PuzzleScript ID to embed.
* `config`: specify configuration. Defaults to:
```javascript
{
	engine: "http://www.puzzlescript.net/js/scripts_play_compiled.js"
}
```
Configuration parameters:
  * `engine`:  Override the engine used (e.g. to keep an archived version locally)

Usage
-----

1. Create a container element for the game
	```html
	<div id="puzzlescript-game"></div>
	```

2. Include CSS
	```html
	<style type="text/css">
		@import url("css/puzzlescript-embed.css");
	</style>
	```

3. Include JavaScript
	```html
	<script src="js/puzzlescript-embed.js" type="text/javascript"></script>
	```

4. Embed the game*
	```html
	<script type="text/javascript">
		PuzzleScript.embed(document.getElementById("puzzlescript-game"), "[your-puzzlescript-game-id]");
	</script>
	```

\* To find your PuzzleScript game's ID, choose the "share" option in the PuzzleScript editor and copy the part labelled `your_puzzlescript_game_id`:

```
http://www.puzzlescript.net/play.html?p=[your_puzzlescript_game_id]
```


Examples
--------

[Threes: The Demake](http://bnhw.co.uk/threes)


License
-------

The MIT License (MIT)

Copyright (c) 2014 Benjamin Davis

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

