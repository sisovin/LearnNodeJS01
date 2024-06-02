# Tutorial 01: Nodejs Understanding
'use strict';
var http = require('http');
var port = process.env.PORT || 5300;

http.createServer(function (req, res) {
    res.writeHead(200, { 'Content-Type': 'text/plain' });
    res.end('Hello World\n');
}).listen(port);

// You should already know:
// HTML, CSS, JavaScript, Node.js, Express, MongoDB, Mongoose, AngularJS, and Git
// possibly experience with other libraries and frameworks like jQuery, Bootstrap, and Angular Material
// and experience with other tools like npm, bower, gulp, and yeoman

// Lesson 1: Introduction to Node.js
// What is Node.js?
// How Node.js differs from Vanilla JavaScript
// 1) Node.js runs on the server, not in a browser (backend not frontend)
// 2) The Console is the terminal window, not the browser console
//    example: go to view -> terminal in Visual Studio 2022
//             then type from the directory where the server.js file is located
//             PS D:\NodeJS\LearnNodeJS>node, then press Enter
// > 2 + 2 (press Enter)
// 4
// PS D:\NodeJS\LearnNodeJS>NodejsWebTest>node server
// > console.log('Hello World') (press Enter)
console.log('Hello World');
// Hello World
// 3) global objects instead of window objects
//    example: go to view -> terminal in Visual Studio 2022
//console.log(global);
// 4) Has common core modules that are still explored
// 5) CommonJS modules are used instead of ES6 modules
const os = require('os');
const path = require('path');
const math = require('./math');
const { add, subtract, multiply, divide } = require('./math');

//console.log(os.type())
//console.log(os.version())
//console.log(os.homedir())

//console.log(__dirname)
//console.log(__filename)


//console.log(path.dirname(__dirname))
//console.log(path.dirname(__filename))

//console.log(path.basename(__dirname))
//console.log(path.basename(__filename))

//console.log(path.dirname(__filename))
//console.log(path.basename(__filename))
//console.log(path.extname(__filename))

//console.log(path.parse(__filename))

console.log(math.add(2, 3));
console.log(math.subtract(3, 2));
console.log(math.multiply(2, 3));
console.log(math.divide(4, 2));
console.log('Split the result');
console.log(add(2, 3));
console.log(subtract(3, 2));
console.log(multiply(2, 3));
console.log(divide(4, 2));

// 6) Missing JS APIs like fetch, local storage, and the DOM
// Lesson 2: Node.js Core Modules like FileSystem module, HTTP, and Path
// File System Module


