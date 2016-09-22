 Step:1
 		window.onload = function() {
      	//set inittial panel state
      	//listen for clicks on tabs
    	}

sample:
</footer>
<script type="text/javascript">
//tabbed panels
    window.onload = function() {
      //set inittial panel state
      //listen for clicks on tabs
    }
</script>
</body>
</html>

 So, window is referencing an object, and the object is the document window itself, meaning the page you're on. Onload is referencing an event. So when you're finished loading. So this is just another way of saying, hey that when the page has finished loading I want to perform a function. I want to execute some code. So essentially now everything in these curly braces is going to execute. It's just some syntax basically. Like the open and close parenthesis that may seem confusing to you. But the curly braces, if you did our chapter on CSS, you're probably used to that. They're used to basically group code together that's going to execute when this function is run. This function's going to run when the page loads. So this is also what we call an anonymous function, meaning it doesn't really have a name, it just performs and does something for us. Okay now, inside of this, I'm just going to do a couple of comments to remind me of what has to happen inside this function. I'm going to type in, set initial panel state. And then on a line below that, I'm going to type in, listen for clicks on tabs

Step: 2
		function displayPanel()


 So I'm going to go down on the next line, and I'm going to type in function and then space and then displayPanel, and notice the P is capitalized there. This is called CamelCase naming. And lower case first word, upper case second word, they're all one big thing. The next thing I'm going to do is open and close my parentheses here. So this function name is not something that already exists inside JavaScript. This is something that I came up with. I invented this. And JavaScript allows up to do that. Essentially, I'm creating a function, I'm giving it a name. Whatever I want to name it. In this case I'm naming it displayPanel. The names of functions typically describe what they do

  Inside of this I'm going to go ahead and do a comment here. I'm going to say respond to tab clicks, so I'm describing the functionality that I want inside of it, and on the next line I'm going to do one more comment. I'm going to type in change panel display and activate tabs. All right, I'll save that. So right now it's not really going to do anything for us but we have sort of what I like to call the skeletons of the functions that are going to complete our tabbed panel for it. One of them will fire when our document loads, and another function, we will fire when we call it.


</footer>
 <script type="text/javascript">
 	//tabbed panels
  window.onload = function() {
    //set inittial panel state
    //listen for clicks on tabs

  function displayPanel() {
 	//respont to tab clicks
 	//change panel display and activate tabs
 }
</script>
</body>
</html>