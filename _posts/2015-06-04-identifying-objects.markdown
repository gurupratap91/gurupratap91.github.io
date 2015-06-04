---
layout: post
title:  "Identifying Objects"
date:   2015-06-04 07:15:06
categories: jekyll update
---

<html>
	<head>
		<title>Identifying Objects</title>
	</head>
<body>
<p>
We started with the simple problem of finding the length of a line. The problem could be solved by making a <i>Line</i> class and implementing a method which would calculate the distance between points(where each point was an array containing x-y coordinates). This was simple. But, what we missed upon was that point was a separate entity which should exist independent of the <i>Line</i> class. Also, the method calculating the length of the line is nothing but the distance between points and it should also belong to the <i>Point</i> class.
</p>

<p>
The problem was further scaled where we had to form rectangles and then squares. We continued with our approach of making rectangles and squares using four points. To verify whether the conditions were satisfied we used our <i>Line</i> and <i>Point</i> classes. The problem was further changed to making squares and rectangles with origin as a point and given sides which were parallel to the axes. The scale for the axes was in "mm". This added the property unit to the sides. We used unit as a string. Other units could be handled using string matching and performing unit conversion. But what was important here to realize was that as we had declared <i>Point</i> as a separate entity, <i>Unit</i> was also supposed to exist independently. Declaring it independently with attributes name and conversion factor (to default unit) made the code more simpler. Unit conversion then became a part of this <i>Unit</i> class. This made the code more readable. Each class had it's own responsibilities. The goal was to give single responsibility to each class.
</p>

<p>
As the problem was extended it made clear how important it is to have separate class for separate entities. We started with the <i>Line</i> class but later on the parameters that we were accepting as arrays and strings turned out to be separate classes. When we added the <i>Unit</i> class for the sides we had to make changes from the <i>Point</i> to the <i>Rectangle</i> and <i>Square</i> classes. This happened because of the dependency of these classes on each other. Frequent changes in the model makes refactoring a tedious task. This shows how important it is to think of a sustainable design while modelling the problem. A good design ensures that the objects involved are identified before hand considering all possible use cases. This makes the process of adding methods and relating these objects quite easy.
</p>
</body>
</html>
