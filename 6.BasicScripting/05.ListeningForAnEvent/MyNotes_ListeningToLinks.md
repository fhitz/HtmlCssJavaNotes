

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
	
	// activate the _first_ one
    displayPanel(tabLinks[0]);
   
    // attach event listener to links using onclick and onfocus, fire the displayPanel function, return false to disable the link
    for (var i = 0; i < tabLinks.length; i++) {
        tabLinks[i].onclick = function() { 
			displayPanel(this); 
			return false;
		}
        tabLinks[i].onfocus = function() { 
			displayPanel(this); 
			return false;
		}
    }
}

function displayPanel() {
	//respond to tab clicks 
	//change panel display and active tabs
}

</script>
</body>
</html>

READ THIS: INSTRUCTION OR EXPLANATION FOR JAVA FUNCTIONS

	Responding to user events is a common task in JavaScript. Perhaps you want to get feedback on a form submission, or update a product display based on the choices that the user made, or in our case, respond to a tab being selected. Listening to and responding to events is a big part of learning JavaScript. So let's see how we can respond to users selecting one of our tabs. So I'm in the 08_05 directory. And it's the next file opened again. And I've already sort of scroll down into our functions. Now, a few things have been added to this, but before we get to that, I want to talk about the concept of responding to an event.

	Basically, essentially you have JavaScript listen for something, and then when that something happens, you have it do something. And usually that's firing off a function, for example. We already have that. Notice that it says, window.onload equals function. So we're listening for the load event. So we're listening for the page to be loaded. When the page loads, we want it to perform this function. So all the code inside of that. So we already kind of have that going on. Now, that's reacting to an event that just sort of happens when the page loads.


displayPanel(tabLinks[0]);
	What if we want to react to a user-based event? So, in this case we want to react to a user actually clicking on one of the tabs. All right. So let's see how we're going to do that. Now if you scroll down a little bit you can see that I've added a few things to our function. The first thing that I've added is right here. Activate the _first_ one. Okay? So here we have the displayPanel, tabLinks, and then 0. So this is the function displayPanel. Would this function's going to be fired immediately when the page loads. We going to do that because we want to set the initial display of the active tab and the active panel.

displayPanel(tabLinks[0]);
	
	To do that we're going to fire off this function. How is this working? Well it's calling the function displayPanel and then it is doing what we calling passing arguments into the function. If you were going to create a function that added two numbers together, you would call the function, like addnumbers, and then in parenthesis you would pass in the two numbers that you wanted to add. In this case we're saying displayPanel and now we need to tell it which tab is the active panel. And for us, the first one's going to be the initial one. All right. So that's where this really weird looking little 0 comes in.
	
	JavaScript starts counting from 0. So think about the number of tabs we have. We have three. So 0 is actually asking for the first one. One would be the second one. Two would be the third one. It's confusing at first, but once you get to using it, it's pretty easy. Now after that, I have another comment that says attach event listener to links using onclick and onfocus. Fire the displayPanel function and returned false to disable to link. So it sounds like there's a lot going on in here. The first thing is I already have a loop built for you so that you don't have to do this.

	Now this is what's known as a for loop. There are a lot of times that we want something to happen to multiple objects in scripting. In this case, we want each one of those tabs to listen for a click. We could write the code to do that for each one of those tabs, but that's going to take us forever. And besides, what if we add more tabs? Right now we only have three, but what if we take a tab away or add more tabs to it? It's much easier if we just have JavaScript go ahead and automatically add it to all of our tabs for us. So here's how it does this. This is called a for loop. It creates an initial variable called i, and it starts at 0.
	
	And then it said hey, as long as i is less than the number of tabLinks, meaning the number of tabs, list items, then take i and add one to it. And then it will execute the code found inside these curly braces. So it's going to go one, two, three, until it runs out of tabs, and then it's going to stop running. So we know that this is going to execute as many times as we have tabs, which is perfect. Okay. So now we need to actually do something here.

displayPanel(tabLinks[0]);


  tabLinks[i].onfocus = function() { 
			displayPanel(this); 
			return false;
		}
	We're basically, now we're going to write what's known as an event listener for our tabLinks. And just like I did last time, I'm going to just paste some code in here, and then ask you guys to pause it. So I'm going to go ahead and paste the code. So, you'll notice that we're creating a function inside of this. It's okay to nest functions inside of functions, nothing wrong with that at all. So what we're saying is, tab links, and then this i. This i is the same variable as this one. So we're starting at 0, and then 1, and then 2. Remember, it's an array, so they count, start counting at 0. So 0 would say the first one, 1 would be the second one, 2 would be the third one, and we know it's going to execute three times.
So we're saying for each of the list items in tabLinks we want to attach an onclick event listener, meaning wait for it to be clicked. When it's clicked we want you to run a function. The function we're going to run is displayPanel. Remember the displayPanel function's right here. What we're going to pass into it is this. Remember up here we're activating the first one by passing that in explicitly. The this keyword, what this does is this references the object that called the function. This is referring to (this).
	
	So it's saying, hey, when I call this function, I want to pass in which tab has been clicked. So it's a very easy way for me to say whoever got clicked. And then finally, we do what's called return false. So we're returning false. And what that's going to do is it's going to disable the link that they click. You remember how, for non-JavaScript users, I made a link that would jump down to that tab? Well, obviously, I don't want it to do that. By saying, return false, I disabled that. Okay, now I mentioned that I want to do this for both onclick and onfocus.
	
	So as soon as I am done with that one I'm going to hit Return. Making sure, by the way, that I'm still in the for loop. And this is where it gets really confusing. You see these ending curly braces? This one pertains to the for loop, this one pertains to the overall function, this one pertains to the tabLinks function. You can't lose sight of those. If you do, and they're out of order, none of your JavaScript will work, so you gotta be really, really careful about this. So outside of my tabLinks onclick function, but still inside my for loop, I'm going to click, and I'll paste one more time. Same thing. And I'm just going to clean that up a little bit. And now instead of onclick I'm going to change this to onfocus. Now, that's just me being thorough. When people click on it with a mouse and onclick registers. Onfocus registers if one of those tabs has focus placed on it any other way. And this is for people that might be using a keyboard for example. Since that's a link, they can tab to that. So, for somebody that might be using assisted technology and maybe can't use a mouse, it's still making sure that my tab panels work for those guys. And you can see the function is doing exactly the same thing. All right, I'm going to go ahead and save that, now I know that was a good bit, but the initial state of our tab panel is now activated and we're now listening for our tabs to be clicked. All we need to do to finish our tabbed panels is respond to the events, and we'll do that next.