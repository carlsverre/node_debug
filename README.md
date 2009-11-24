Node Debug
==========

A HTTP based console and object explorer for [node.js](http://nodejs.org/).

Its like a REPL for a node app in the browser.


Usage
-----

Include the following in your project:

    var debug = require("debug.js");
    debug.listen(8080);

Example:

    $ /usr/local/bin/node server.js

Browse to: http://127.0.0.1:8000/ for http
Browse to: http://127.0.0.1:8080/ for debug

var view = {
	  title: "Main Page",
	  calc: function() {
		return 2 + 4;
	  }
	}

debug.log(view);

Click on objects to expand properties.
