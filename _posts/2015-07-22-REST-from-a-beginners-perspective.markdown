---
layout: post
title:  "REST from a beginner's perspective"
date:   2015-07-22 02:10:06
categories: jekyll update
---

<html>
	<title>
		<head> REST from a beginner's perspective </head>
	</title>

<body>
<p>
REST stands for Representation State Transfer which is an architectural style for the web applications. What REST focuses on is a web which has a rationale to support it in becoming scalable. It emphasizes on better user perceived performance, separation of concerns and provide generic interfaces for better communication between components. In a RESTful architecture the request and response objects of queries are representations of data and not the original data.
</p>
<p>
Any form of information that can be named are called resources in REST. A resource is a mapping to a set of entities which and represent their state which varies with time. This means that they can be both static as well as dynamic depending upon the semantics of the mapping. For example, "User's favorite song" is a mapping which changes with time whereas "Composer of the song Black" is a mapping which is static. REST allows us to define identifiers for these resources instead of defining documents identifiers which was done previously. Defining document identifiers meant that it would have to be changed as soon as the data in the documents changed. Resource identifiers allows us to identify the concept rather than the actual content. However, it then becomes our responsibility to ensure that the identifier chosen does correspond to intended resource. 
</p>
<p>
To illustrate how REST can be applied let's see how Rails works in RESTful manner. Rails identifies data objects like files, images, videos, etc. by the term <i> resource </i>. These resources are instances of the model they belong and have a controller associated with them for their manipulation. The resources are identified by uniform identifiers which makes URLs simpler. The controller includes the <i>index,edit and new </i>actions along with the CRUD operations. The action to be performed is identified by understanding the query which is a combination of HTTP verbs(GET, POST, PUT and DELETE ) and the URI specified. These are known as RESTful routes which are created when the resource is first generated. Along with these routes PATH functions and URL functions like <i>resource_path</i> and <i>resource_url</i> are also created. These PATH and URL functions are helpful in adding links and redirects respectively. REST allows representations of resources to be sent across easily by just adding the formats in the URI specified in the respond_to blocks.  
</p>
<p>
To get a thorough idea of the constraints involved in REST you can go through the <a href="http://www.restapitutorial.com/lessons/whatisrest.html#"> What is REST? </a> or the document where these constraints were first communicated by Roy Fielding in his doctoral dissertation (see<a href="http://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm"> http://www.ics.uci.edu/~fielding/pubs/dissertation/rest_arch_style.htm)</a>  
</p>
</body>
</html>
