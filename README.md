# CheatSheet-for-backend



const express = require("express");
const app = express();
const ejs = require("ejs")
const mongoose = require("mongoose")
const bodyParser = require("body-parser")

app.set('view engine', 'ejs');
app.use(bodyParser.urlencoded({ extended: true}));
app.use(express.static("public"));

mongoose.connect("mongodb://localhost:27017/(DATABASE NAME)", {useNewUrlParser: ture});

//TODO

app.listen(3000,function(){
    console.log("Server running on port 3000")
});
