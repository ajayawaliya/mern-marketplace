# mern-marketplace
// var express = require('express');
// var app = express();
// app.get('/',function(req,res) {
//   res.send('Hello World!');
// });
// var server = app.listen(4000, function() {console.log("Server is running")});


var express = require('express');
var app = express();
app.route('/Students').get(function(req,res) {
  res.send ("Welcome to student information");
});
app.route('/Admin').get(function(req,res) {
  res.send ("Welcome to admin page");
});
app.route('/').get(function(req,res) {
  res.send ("Welcome to home page");
});
var server = app.listen(4000, function() {console.log("Server is running") });
