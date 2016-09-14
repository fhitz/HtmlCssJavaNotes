

  1st step: open the file 'link.htm'

      <p>Link to the <a href="same.htm" title="same.htm">same.htm</a>page, in the same directory</p>
    
  So in order to get to that page from here, I have to go into the info directory. And then into the extras directory. And then finally, resource.html All right. So I need to create another anchor element here.

  2nd step: from  'links.htm' to 'resources.htm'
    
    <p>Link to the<a href="info/extra/resource.htm" title="down two directories">resources.htm</a> page, in a nested directory</p>

  3rd step: about.htm

    <p>Link to the <a href="../links.htm" title="up a directory">links.htm</a> page, up one directory</p>
    <p>Link to the <a href="extras/resources.htm" title="down a directory">resources.htm</a> page, down one directory</p>

        Tips bonus:     ../
             essentially tells the browser to go up one directory.

  4th step: from  'resources.htm'  to  'links.htm'

    <p>Link to the <a href="../about.htm" title="up a directory">about.htm</a> page, up one directory</p>
    <p>Link to the <a href="../../links.htm" title="up two directories">links.htm</a> page, up two directories</p>

          
  