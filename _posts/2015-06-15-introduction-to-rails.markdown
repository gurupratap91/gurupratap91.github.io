---
layout: post
title:  "Introduction to Rails"
date:   2015-06-15 00:45:00
categories: jekyll update
---

<html>
	<head>
		<title>Introduction to Rails</title>
	</head>
<body>
<p>
Rails is a web framework of Ruby. A framework is a set of conventions which make the process of writing applications easier. It is based on the pattern of <i>Models Views and Controllers</i> popularly known as the MVC pattern. MVC allows us to distribute the responsibilities to each of these modules. Models deal with the interactions with the database. They are responsible for creating tables in the database or to perform any kind of queries from the database. Views contain the formatting of the data which is to be displayed to the user. At times they also provide data to be written to the database e.g. in case of form submissions. Controllers are responsible for the actions to be taken for different use cases. They contain the actions that are to be performed when requests are made from the web server. What connects the actions in the controllers to different views are called routes. As the name suggests they define which action is responsible for the rendering of which view.
</p>
<p>
I worked on rails to set up a blog using the <a href="http://guides.rubyonrails.org/getting_started.html">rails guide</a>. It allows user to publish articles with the fields containing a <i>title</i> and <i>text</i>. Used the <i>rspec-rails</i> gem to write tests for the models, controllers and routes(haven't written tests for the views yet). Rails encourages to have a RESTful architecture which makes identifying resources and performing operations on them easier. In particular, this property of Rails make routing easier and everything can be done on the basis of names. 
</p>
<p>
Rails focuses on some philosophies which makes development and maintainance of applications an easy task.
</p>
<p>
Rails follows the philosophy of <i>CoC(Convention over Configuration)</i> which makes the developer's task easier. The more you are into following the conventions that the language has the lesser amount of code you have to write. For example, generating a model <i>Article</i> will automatically map it to the <i>articles</i> table in the database. The attributes are added in the <i>articles</i>table and automatically mapped to the <i>Article</i> model. There's no need to mention the attributes of the table in the <i>Article</i> class explicitly. This is how convention helps us save time when compared to the situation where you would have to manually configure the database as well.
</p>
<p>
It also encourages <i>FMSC(Fat models, skinny controllers)</i>. It means that most of the application logic should be placed within the model while leaving the controller as light as possible. It says that the non response related logic should go into the model. It also makes such code reusable in other related contexts.
</p>
<p>
It also emphasizes on <i>DRY(Don't Repeat Yourself)</i>. Keeping the code DRY means you whenever possible, reuse as much code as possible rather than duplicating similar code in multiple places. This prevents inconsistency in code when changes are made. For example, using <i>partials</i> to clean up duplication in views. The view partial <i>_form.html.erb</i> helped in keeping the identical code being used in <i>new.html.erb</i> and <i>view.html.erb</i> in the same place. This sums up my understanding of concepts related to Rails that I have learnt until now.
</p>

<a href="https://github.com/gurupratap91/blog">Click here</a> to take a look at the github repository of the blog.
</body>
</html>
