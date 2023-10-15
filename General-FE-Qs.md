#General Frontend Questions

<ul>
<li><b> REST - </b> REST stands for Representational State Transfer. </li>
<li><b>What is a REST API?</b> An API is an application programming interface, which is a software-to-software interface that allows otherwise separate applications to interact and share data. In a REST API, all data is treated as resources, each one represented by a unique uniform resource identifier (URI). </li>

<li> <b>What are some of the main benefits of REST web services?</b> The learning curve is very simple because it works based on HTTP protocols
Supports several data transfer technologies such as ext, XML, JSON, image, etc.
Has no predefined contract between server and client, so loosely coupled implementation
REST is a very lightweight protocol
REST methods can be easily tested in the browser</li>
<li><b>What is Cross-Site Scripting (XSS)?</b>Cross-Site Scripting (XSS) is an attack that occurs when an attacker uses a web application to send malicious code to a different end-user. This code is usually in the form of a browser-side script.
The page provided by the server when someone requests it is unaltered. The XSS attack exploits weaknesses in the page that include a variable submitted in a request to show up in the raw form in the response. The page will only display what was sent along with this request.</li>
<li><b>What is load balancing? </b>Load balancing is distribution of all the incoming network traffic all across the backend servers. 
</li>
<li><b>NPM</b> - Node Package Manager</li>
<li><b> What is scope in JavaScript?</b>In JavaScript every function has its own scope. It is basically a collection of rules for how variables are accessed and variables itself. Globally scoped variables can be used throughout the app bc they are not assigned within a function. Locally scoped are only to be used inside of the function</li>
 <li><b>What is a CDN?</b> A content delivery network (CDN) is a system for delivering content to users based on geographic location. CDNs can deliver websites, software applications, and other types of digital content.</li>
 <li><b>What is AJAX?</b> AJAX is a web development technique for creating asynchronous web applications. AJAX allows you to create dynamic, responsive web applications that can be updated without reloading the page.</li>
 <li><b>What are the differences between HTML and XHTML?</b> HTML is the standard markup language for creating web pages. XHTML is a stricter and more well-defined version of HTML. It's frequently used for formatting more complex documents within a stated taxonomy.

HTML code:

```HTML
<!DOCTYPE html>
<html>
<body>

<h1 style="background-color: red;">Hello World!</h1>
<p>This is a paragraph.</p>

</body>
</html>
```

XHTML code:
```HTML
<?xml version="1.0" encoding="UTF-8"?>
<?xml-stylesheet type="text/css" 
    href="http://www.w3.org/MarkUp/style/xhtml2.css"?>
<!DOCTYPE html PUBLIC "-//W3C//DTD XHTML 2.0//EN"
    "http://www.w3.org/MarkUp/DTD/xhtml2.dtd">
<html xmlns="http://www.w3.org/2002/06/xhtml2/" xml:lang="en"
    xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
    xsi:schemaLocation="http://www.w3.org/2002/06/xhtml2/
        http://www.w3.org/MarkUp/SCHEMA/xhtml2.xsd"
>
<head><title>Hello World!</title></head>
<body><p>This is a paragraph.</p></body>
</html>
```
</li>
 <li><b>What is responsive design?</b>Responsive design is a web development technique that creates websites compatible with multiple devices with different screen sizes. Responsive websites are designed to look good on both desktop and mobile devices.</li>
</ul>
<ul>
<li><b>How would you optimize a website's performance?</b>First, you should make sure that your code is minified and compressed. This reduces the size of your files, which makes them faster to download. 

Second, you should use caching wherever possible. This stores frequently used files locally, so they don't need to be downloaded every time a user visits your site. But don’t overdo it, or your site won’t be as dynamic as you want — it won’t update as reliably.

Finally, you should use a content delivery network (CDN). This distributes your files across multiple servers, so users can download them from their respective locations. </li>
<li><b>What are some common issues that you have faced with cross-browser compatibility?</b>Some of the most common issues with cross-browser compatibility are different browsers rendering CSS differently, different browsers supporting different HTML and CSS features, and different browsers having different levels of support for standards. This is particularly difficult as many browsers differ depending on the platform, and the platform differs so widely; someone can open Chrome OS on a smart fridge today.</li>
<li><b>process for debugging code: </b>
<ul>
<li><b>Understand the Problem:</b>Begin by gaining a clear understanding of the problem you’re trying to solve.</li>
<li><b>Review the Requirements or Specifications:</b>Review the requirements or specifications and ensure that you know what the expected behavior of your code should be.</li>
<li><b>Reproduce the Issue:</b>Try to reproduce the problem consistently. Identify the specific inputs or conditions that trigger the bug. Reproducing the issue reliably is crucial for understanding and fixing the problem.</li>
<li><b>Isolate the Problem:</b> Narrow down the scope of the issue by identifying the specific part of your codebase that is causing the problem. This can involve using debugging tools, print statements, or divide-and-conquer techniques. By isolating the problem, you can focus your debugging efforts effectively.</li>
<li><b>Check for Obvious Errors:</b> Review your code for any obvious errors, such as typos, syntax mistakes, missing or incorrect function arguments, incorrect variable assignments, or incorrect algorithmic logic. Often, these simple errors can cause unexpected behavior.</li>
<li><b>Utilize Debugging Tools: </b>Utilize the various debugging tools provided by your programming environment or integrated development environment (IDE). These tools can include breakpoints, stepping through code line by line, watching variables, examining the call stack, and inspecting the state of your program at runtime. These tools can help you observe the program’s behavior and identify issues.</li>
 <li><b>Print Statements:</b> Place print statements strategically in your code to output the values of variables, function calls, or specific checkpoints. This can help you understand the flow of execution and identify problematic areas.</li>
 <li><b>Examine Error Messages and Logs: </b>Carefully read any error messages or warnings that are generated by your code. Understand what they are telling you, and trace back to the source of the problem based on the information provided.</li>
  <li><b>Research:</b>If you’re unable to identify the issue on your own, leverage external resources such as documentation, forums, or online communities. Search for similar issues or error messages that others have encountered and solved. Often, someone else has encountered a similar problem and can provide helpful insights or solutions.</li>
</ul>
</li>
<li><b>server-side vs client-side rendering:<br> </b>Server-side rendering (SSR) and client-side rendering (CSR) are two different approaches to rendering web content and delivering it to the user’s browser.
<ul>
<li><b>Server-Side Rendering (SSR):</b><br>In server-side rendering, the web server processes the request and generates the complete HTML content on the server itself. The server executes the necessary code, fetches data from databases or external APIs, and generates the HTML markup that represents the final web page. This complete HTML response is then sent to the client’s browser, where it is rendered and displayed.</li>
<li><b>Advantages of SSR</b></li>
<li><b>Improved Initial Page Load Time:</b> Since the server sends the pre-rendered HTML content, the user sees the content sooner.</li>

<li><b>SEO Friendliness:</b> Search engine bots can easily crawl and index the pre-rendered HTML content, thus enhancing search engine visibility.</li>

<li><b>Disadvantages of SSR</b></li>

<li><b>Increased Server Load:</b> The server has to handle the rendering process for each request, which can be resource-intensive.</li>

<li><b>Limited Interactivity:</b> Most interactivity requires additional round-trips to the server, which can slow down the user experience.</li>
</ul>
<ul>
<br>
<li><b>Client-Side Rendering (CSR):</b><br> In client-side rendering, the web server sends a minimal HTML document to the client’s browser, typically including some basic JavaScript and CSS files. The browser then downloads these files and executes the JavaScript code. The JavaScript code is responsible for fetching data from APIs, thus manipulating the DOM (Document Object Model), and rendering the content dynamically on the client side.</li>
<li><b>Advantages of CSR</b>
<ul>
<li><b>Enhanced Interactivity:</b> With the processing happening on the client side, applications can provide highly interactive experiences without needing to request data from the server for every user action.</li>
<li><b>Reduced Server Load:</b>The server primarily serves static files, reducing the server load and making it more scalable.</li>
</ul>
</li>
 <li><b>Disadvantages of CSR</b>
 <ul><li><b>Slower Initial Page Load:</b>Since the initial HTML content is minimal, the browser needs to download JavaScript and CSS files and execute the JavaScript code before rendering the content, thus resulting in a slower initial page load.</li>
 <li><b>SEO Challenges:</b>Search engine bots may not effectively crawl and index dynamically generated content, thus potentially impacting search engine visibility.</li>
 <li>Although techniques like server-side rendering of critical pages or pre-rendering can mitigate this issue. It’s worth noting that hybrid approaches, such as server-side rendering with client-side hydration (where the server sends pre-rendered content and the client-side JavaScript takes over to enable interactivity) are a popular choice for combining the advantages of both SSR and CSR. The choice between SSR and CSR depends on various factors like the type of application, performance requirements, SEO consideration, and user experience goals.
 </li></ul>
 </li>

</ul>
 <li><b>Prototype Design Pattern: </b>The Prototype Pattern creates new objects. But the peculiarity is that instead of creating non-initialized objects, it returns objects that are initialized with values ​​ copied from a prototype - or sample - object.

One example is the initialization of business objects with values ​​that match the default values ​​in the database. Classical languages ​​rarely use the Prototype pattern, but JavaScript being a prototypal language uses this pattern in the construction of new objects and their prototypes.</li>
 <li><b>Content Security Policy: </b>Content Security Policy (CSP) is an HTTP header that allows operators to monitor and control where resources can be loaded onto their website. Using this header is one of the best ways to prevent cross-site scripting (XSS) vulnerabilities. Since there are difficulties with retrofitting CSPs on all existing websites, CSP is a must for all new websites, and it is highly recommended to implement CSPs on all existing high-risk sites.

The biggest benefit of CSP is disabling the use of unsafe-inline JavaScript. Inline JavaScript means that data that users enter incorrectly on the site can generate code that will be interpreted by the browser like JavaScript. By using CSP to disable inline JavaScript, you can effectively eliminate almost all XSS attacks against your site.</li>
<li><b></b></li>
<li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
 <li><b></b></li>
</ul>
