node_debug
==========

An asynchronous HTTP based console and object explorer for node.js [node.js](http://nodejs.org/).


Usage
-----

var sys = require('sys'),    
	http = require('http'),   
	debug = require("./node_debug/debug");

/* start debugging on host:8080 */
debug.listen(8080);

http.createServer(function (req, res) {
  setTimeout(function () {
    res.sendHeader(200, {'Content-Type': 'text/plain'});
	res.finish();
  }, 2000);
}).listen(8000);

/* server started */	
sys.puts('Server running at http://127.0.0.1:8000/');


Browse to: http://127.0.0.1:8000/ for http
Browse to: http://127.0.0.1:8080/ for debug

