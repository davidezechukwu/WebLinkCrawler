# WebLinkCrawler

<h2>Project Structure</h2>
<ul>
  <li>App\Program.cs</li>  
  <li>App\AppTest</li>  
  <li>App\AppTest\ProgramTest.cs</li> 
  <li>App\Publish</li> 
  <li>App\Publish\program.exe</li> 
  <li>App\Publish\program.exe</li> 
</ul>
<h2>Runing</h2>
<ul>
  <li>Navigate to the directory ./App/publish</li>  
  <li>Run program.exe [domain] [number of pages to index]</li> 
  <li>Alternatively just run program.exe for the command line options</li> 
</ul>
<h2>Testing (Unit Tests uses MSTest)</h2>
<ul>
  <li>Navigate to the directory ./app/publish</li>  
  <li>Run [PATH TO vstest.console.exe] programtest.dll</li> 
     For Example: "D:\Program Files (x86)\Microsoft Visual Studio\2017\Enterprise\Common7\IDE\Extensions\TestPlatform\vstest.console.exe" programtest.dll
  <li>Alternatively Load the solution or projects in Visual Studio and carry out the tests from  the IDE</li>
</ul> 

<h2>Building:</h2>
The Solution and projects were built using Visual Studio Enterprise 2017 hence Visual Studio or Visual Code is required.

<h2>ToDo</h2>
<ul>
  <li>The emphasis is on web crawling hence, for simplicity of code, there is no threading involved - the use of thread would speed up the crawl process as the code is blocked each time a web request is made</li> 
  <li>The emphasis is on web crawling hence, for simplicity of code, there is no use of interfaces or abstract base classes or Object Orientation, all the crawl logic is located on one static class</li> 
  <li>There is a limit to the number of pages that could be indexed</li> 
  <li>There is no handling of sub-domains</li> 
  <li>Test coverage might not be 100%</li>  
  <li>No design patterns were used, however I could have used the strategy pattern to implement services for generating either XML, TEXT or JSON from the crawled page link</li>
</ul>
