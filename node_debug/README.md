node_debug
==========

An asynchronous HTTP based console and object explorer for node.js [node.js](http://nodejs.org/).


Usage
-----

Include the following in your project:

    var debug = require("debug.js");
    debug.listen(8080);


Browse to: http://127.0.0.1:8000/ for http

Browse to: http://127.0.0.1:8080/ for debug


Example:

var view = {
	  title: "Main Page",
	  calc: function() {
		return 2 + 4;
	  }
	}

debug.log(view);

Click on objects in log view to expand properties.



FEATURES

History
Snippets 
Multiple-Clients