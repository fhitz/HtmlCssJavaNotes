Step: 1 

	// declare globals to hold all the links and all the panel elements
<script type="text/javascript">
var tabLinks;
var tabPanels;
</script>
 
 DOM:
 Using the DOM or Document Object Model. The DOM is a standardized way of referencing page elements in HTML documents. The elements are described as a tree with parent nodes at the top. And child nodes branching off in a sequence. So for this document, for example, the body element would be seen at the top of the tree.

And then this header would be an immediate child node off of that. The dom not only describes this tree, but also gives us methods for traversing and accessing these elements programmatically.


The var keyword right here var. Creates a new variable and then I name those variables whatever I want, tablinks and tabPanels in this case. So essentially I'm creating variables to hold all of my tabs and another variable to hold all of my panels. Because I'll need to control them through scripting so I need some way of referencing those items. Now what is a variable, well a variable is anything I want it to be.

</footer>
<script type="text/javascript">
//tabbed panels

// declare globals to hold all the links and all the panel elements
var tabLinks;
var tabPanels;

</script>
</body>
</html>


Step:2
	
 So the first comment sort of gives us a little idea. When the page loads, grab the Li elements. Now those list item elements are the actual tabs themselves. If you remember, if I scroll up and look at the actual structure of our tabs. You can see that each of the tabs is inside of a list item element. So we are creating a variable that's storing all of those in that. Now, that's referred to as an array. Because we're storing multiple objects inside a single variable. It's not that important but it's interesting for you to hear the terminology.

 So we're creating an array. And storing those list items inside of that. So what we're doing is we're saying tab links equals. Equals is what we call an assignment operator. We're assigning a value. So we're taking the variable that we created up here and then we're saying, hey. That variable that we created, let’s put something in the pickle bucket. So were saying equals and then we have our document object model being used. So we’re saying Document, that’s the current open document, and then we have .getElementById, this is what’s called dot notation.

 And this is a way of scripting that basically lets us reference objects and use what we call methods to manipulate those objects. So, this object is the document itself, and then we're using a method called get element by id. Now this is built, or baked into JavaScript, okay. So, it's part of the document object model. We're saying get element by id tabs. Now remember we have all those ids up here. Let me show you what this is referencing. We have a div with an id of tabs. So essentially we're referencing this element, okay? Now below that we have another dot notation and now we're saying, get elements plural by tag name. List item. So, essentially, if I were to, say this in pure English. I would say, hey, go in the open document, find an element that has an ID of tabs. Inside that, retrieve any elements that have a tag name of list item, or give me all the list items inside of that. So that's exactly what this is doing. And it's storing them in the variable tablinks. 

So go inside containers, find all the divs and I'm storing these inside tabPanels. So again, tab links has all of the lis, list items, the individual tabs tab panels as the individual divs that are the panels themselves. So, so far we've created two global variables. And then used the document object model to store all of our tab widget elements that we'll need to control through Java Script. So next, we're going to need to activate our initial tab. And then react when that tab is clicked.

</footer>
<script type="text/javascript">
//tabbed panels

// declare globals to hold all the links and all the panel elements
var tabLinks;
var tabPanels;

window.onload=function() {
    // when the page loads, grab the li elements
    tabLinks = document.getElementById("tabs").getElementsByTagName("li");
	// Now get all the tab panel container divs
	tabPanels = document.getElementById("containers").getElementsByTagName("div");
}

function displayPanel() {
	//respond to tab clicks 
	//change panel display and active tabs
}

</script>
</body>
</html>