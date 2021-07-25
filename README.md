
# Traffic Sign Recognition

Nowadays,	there	is	a	lot	of	attention	being	given	to	the	ability	of	the	car	to	drive	itself.	One	of	
the	many	important	aspects	for	a	self	driving	car	is	the	ability	for	it	to	detect	traffic	signs	in	order	
to	provide	safety	and	security	for	the	people	not	only	inside	the	car	but	also	outside	of	it.
The	traffic	environment	consists	of	different	aspects	whose	main	purpose	is	to	regulate	flow	of	
traffic,	 make	 sure	 each	 driver	 is	 adhering	 to	 the	 rules	 so	 as	 to	 provide	 a	 safe	 and	 secure	
environment	to	all	the	parties	concerned.

The	main	objective	of	our	project	is	to	design	and	construct	a	computer	based	system	which	can	
automatically	detect	the	road	signs	so	as	to	provide	assistance	to	the	user	or	the	machine	so	that	
they	can	 take	appropriate	actions

## Approach

  
We have used	convolutional	neural	networks	(CNN)	to	classify	the	traffic	signs	and	we	used	color	
based	segmentation	to	extract/crop	signs	from	images.
We deployed the model on web using flask,  Html/css and java script .
## Demo
Ig
<img src="https://user-images.githubusercontent.com/63184114/126889551-f89d3ea8-4656-4985-8b10-c1f36717b553.png" width="30%">.
  
## Documentation

The	problem	of	traffic	sign	recognition	is	twofold:


Extracting	a	potential	traffic	sign	from	an	image.
Traffic	 signs	 are	 designed	 such	 that	 they	 appear	 unique	 and	 easily	 identifiable	 to	 the	
human	eye.	Traffic	signs	in	the	United	States	of	America are	of	3	main	colors:	Red,	White,	
and	 Yellow.	 Other	 colors	 like	 orange	 and	 blue	 are	 also	 used.	 In	 our	 approach	 we	
concentrate	on	Red,	White,	and	Yellow	traffic	signs. 

We cropped the image to the area of interest where the focus is only on the signs.
Once	 we	 have	 refined the set	 of	 areas	 of	 interest, we	 use	 the	 convolutional	 neural	
network	which	we	are	going	to	build	in	the	next	step	to	predict	the	type	of	this	sign	(or	if	
it	is	not	a	sign).	

The data set was collected from kaggle , which have about 43 diffrent classes
. The	
test	set	was	obtained	by	splitting	the	whole	dataset	into	80%	train	data	and	20	%	validation	and	
test	data.
Once	the	CNN	has	been	trained, it	is	used	to	predict	the	sign	of	the	contours obtained. 

`Accuracy with the test data : 0.9403 `

![App Screenshot](https://user-images.githubusercontent.com/63184114/126889414-54d10cc1-d713-4eb5-9c09-14f5e5ce4418.png)

