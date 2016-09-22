<!-- always compare this folder to finished_files folder -->

how to make DIV ID="tabContainer"

READ THIS:
Now remember, earlier in the course, we talked about how divs allow us to group content together without having to have an explicit semantic meaning. So we have a lot of tabs going on here and divs are extremely useful for grouping this type of content. The first thing we have is a div that's with an id of tabContainer. Now the use of id's here is really important, because JavaScript allows us to do a lot of different things. One of the things that allows us to do is go through our document and retrieve elements or reference elements based on certain attributes. One of the attributes that it can reference is the id attribute. So the id attribute is unique. Meaning, I can only use it once per page. So if I give an id of tabContainer, I know in scripting that, that is the only element that I could be referring to. So, this has a div id of tabContainer and that surrounds both the tabs and then the panels themselves. So the tabs are in another div with the id of tabs. I have three of those, tabs 1, 2 and 3. And notice that they are linking down to the ids of the panels below them. And then I just have the text that displays HTML, CSS and JavaScript. Now below the tabs, I have another div with an id of containers. This wraps all of the actual panels themselves, panels 1, 2 and 3. Inside of that, I have the individual panels. Notice that they have the id of tabPanel1. We have tabPanel2 and we have tabPanel3. And each of these divs surrounds an h4 followed by paragraphs that have descriptive text.

Sample:

<div id="tabContainer">
    <div id="tabs">
      <ul>
        <li id="tab1"><a href="#tabPanel1">HTML</a></li>
        <li id="tab2"><a href="#tabPanel2">CSS</a></li>
        <li id="tab3"><a href="#tabPanel3">Javascript</a></li>
      </ul>
    </div>
    <div id="containers">
      <div id="tabPanel1">
        <h4>HTML</h4>
        <p><strong>Hypertext Markup Language.</strong> Controls the structure and semantics of web pages. Tags are used to mark up elements and denote content type. Although HTML does contain some presentational elements, it consists primarily of logical tags that identify content or provide information on content hierarchy.</p>
        <p>HTML also allows for images and media such as video to be embedded as content on pages. This is usually referred to as replaced content, as the HTML tag will refer the user agent to fetch an external resource.</p>
      </div>
      <div id="tabPanel2">
        <h4>CSS</h4>
        <p><strong>Cascading Style Sheets.</strong> Controls the visual presentation of page elements. It is responsible for page layout, color, typography, and element dimensions. Recent additions to CSS have included transforms and animations, which have greatly expanded the capabilities of CSS and the effects that can be controlled through it.</p>
        <p>CSS is a presentational language, meaning that it's syntax references page elements, and then assigns values to the visual properties of those elements. Although the basic syntax is easy to learn there are a considerable amount of properties and values to learn, as well as which element types they can apply to.</p>
        <p>The "cascading" nature that CSS derives its name from indicates how styles are applied by user agents. Since styles can be applied from multiple sources, there are rules that control when styles are applied and how to resolve conflict. Understanding the cascade is a critical part of controlling site-wide styles efficiently.</p>
      </div>
      <div id="tabPanel3">
        <h4>Javascript</h4>
        <p><strong>JavaScript.</strong> Controls the behavior of page elements and is used to create interactive widgets, facilitate user interaction, control the browser, or a host of other functions. Javascript is a programming language, and its syntax is arguably the most difficult to learn of the three core languages. Page elements are accessed through the <strong>DOM</strong> (Document Object Model) and then manipulated through <strong>events</strong> and <strong>functions</strong>.</p>
        <p>Because the code is executed within the browser and not on a web server, Javascript is often referred to as a "client-side" scripting language. This functionality makes Javascript faster than many other scripting choices, and capable of providing instant feedback or results to the user.</p>
 <p>Over the years many Javascript frameworks and libraries have been developed to extend the capabilities of Javascript and make it faster to write. The success of libraries like jQuery have led to an explosion of Javascript development and have solidified it as the <i>de facto</i> scripting language for the web.</p>
      </div>
    </div>
  </div>



JAVACRIPT:

added tags: script or javascript
javascript comment: //

<script type="text/javascript">
//table
</script>

where to put the script tag: see sample below

sample:
<footer role="contentinfo">
  <p>&copy; <a href="http://www.lynda.com" title="lynda.com" target="_blank">lynda.com</a> | follow me and lynda.com on Twitter! <a href="https://twitter.com/jameswillweb" title="Follow me on Twitter">@jameswillweb</a> <a href="https://twitter.com/lynda" title="Follow lynda.com on Twitter">@lynda</a></p>
</footer>

<script type="text/javascript">
//table                
</script>

</body>
</html>


<!-- always compare this folder to finished_files folder -->