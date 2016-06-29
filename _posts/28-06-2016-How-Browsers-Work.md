There are several browsers used on both desktop and mobile device today. These include: *Chrome *Firefox *safari *Opera

![Popular browsers](http://markmwaura.github.io/images/browsers.jpg)

### Main function of a browser
The main function of a browser is to present the web resource you choose, by requesting it from the server and displaying it in the browser window. The resource is usually an HTML document, but may also be a PDF, image, or some other type of content. The location of the resource is specified by the user using a URI (Uniform Resource Identifier).

Common User interface elements of a Browser:

1.Home button that takes you to your home page

2.Bookmarking Options

3.Back and Forward buttons

4.Address Bar for inserting URI

5.Refresh and Stop butoons for refreshing or stopping the loading of current pages/documents
The browsers high level structure The browsers main components are :

1.The User Inteface : This includes the address bar, back/forward button, bookmarking menu, etc. Every part of the browser display except the window where you see the requested page.

2.The Browser Engine : It manages actions between the UI and the rendering engine.

3.The Rendering Engine: This is responsible for displaying requested content content.For example if the requested content is HTML, the rendering engine parses HTML and CSS, and displays the parsed content on the screen.

Different browsers use different rendering engines: Internet Explorer uses Trident, Firefox uses Gecko, Safari uses WebKit. Chrome and Opera (from version 15) use Blink, a fork of WebKit(an open source rendering engine which started as an engine for the Linux platform and was modified by Apple to support Mac and Windows).

### The main Flow

The rendering engine will start getting the contents of the requested document from the networking layer. This will usually be done in 8kB chunks.The rendering engine will start parsing the HTML document and convert elements to DOM nodes in a tree called the "content tree". The engine will parse the style data, both in external CSS files and in style elements. Styling information together with visual instructions in the HTML will be used to create another tree: the render tree.
The render tree contains rectangles with visual attributes like color and dimensions. The rectangles are in the right order to be displayed on the screen.
After the construction of the render tree it goes through a "layout" process. This means giving each node the exact coordinates where it should appear on the screen. The next stage is painting–the render tree will be traversed and each node will be painted using the UI backend layer.
It's important to understand that this is a gradual process. For better user experience, the rendering engine will try to display contents on the screen as soon as possible. It will not wait until all HTML is parsed before starting to build and layout the render tree. Parts of the content will be parsed and displayed, while the process continues with the rest of the contents that keeps coming from the network.


4.Networking: This is responsible for network calls such as HTTP requests, using different implementations for different platform behind a platform independent interface.


5.UI backend: This is used for drawing basic widgets like combo boxes and windows. This backend exposes a generic interface that is not platform specific. Underneath it uses operating system user interface methods.


6.Javascript Interpreter:Used to parse and execute javascript code.


7.Data storage: This is a persistence layer. The browser may need to save all sorts of data locally, such as cookies. Browsers also support storage mechanisms such as localStorage, IndexedDB, WebSQL and FileSystem.

It is important to note that browsers such as Chrome run multiple instances of the rendering engine: one for each tab. Each tab runs in a separate process. 