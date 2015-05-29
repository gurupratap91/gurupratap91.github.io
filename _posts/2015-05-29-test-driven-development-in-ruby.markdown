---
layout: post
title:  "Test Driven Development in Ruby"
date:   2015-05-29 11:10:06
categories: jekyll update
---

<html>
	<title>
		<head> Test Driven Development in Ruby </head>
	</title>

<body>
<p>
Test Driven Development (TDD) focuses on testing the logic rather than the previously existing code. Ruby has libraries(e.g. <a href="http://rspec.info/">Rspec</a>) to support TDD and ‘rake’ to automate the process of running these tests on the code written. Organising the project in a prescribed manner makes this entire process very easy and understandable for a new person as well. Let’s see how the directory is organised.
</p>

<p>
There are four things that you need to keep under consideration : 
<ol>
	<li>/lib directory - This stores the implemented logic</li>
	<li>/test directory - This stores the tests written for the logic (/spec in case of Rspec library)</li>
	<li>Gemfile - Stores the dependencies involved for the code to run</li>
	<li>Rakefile - This stores the operation that you need to perform on the source code</li>
</ol>
</p>

<p>
The above directory structure allows you to setup any project, such that it follows TDD and remains machine independent. It breaks the code into desired modules and also applies the concept of single responsibility e.g. the /lib directory only deals with the logic. In the long term it makes refactoring easier. This is possible because the changes made just have to make sure that the previously written tests are passed.
</p>

<p>
A typical project can be set up in the following way:
<ol>
	<li>Create a project directory : <i>mkdir project</i></li>
	<li>Move to the project directory : <i>cd project</i></li>
	<li>Create /lib directory : <i>mkdir lib</i></li>
	<li>Create /spec directory(for Rspec library) : <i>mkdir spec</i></li>
	<li>Initialize bundler to create Gemfile : <i>bundle init</i></li>
	<li>Add the required gems to the Gemfile : e.g. add line <b><i>gem 'rspec’</i></b> to add the gem rspec</li>
	<li>Initialize the Rspec gem to create the helper files: <i>rspec –init</i></li>
	<li>Create the Rakefile to define the tasks needed to be performed on the code(check the example to see the content of a rakefile) : <i>vim Rakefile</i></li>
</ol>
</p>

<p>
To go through an example project created using the above rules<a href="https://github.com/gurupratap91/line.git"> click here</a>.
It contains a project which calculates the length of a line given the starting and the end points of the line.
</p>

