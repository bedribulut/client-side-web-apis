- APIs are programming features for manipulating different aspects of the browser and operating system the site is running on, or manipulating data from other web sites or services.
introduction to web APIs
- APIs in client-side JavaScript: browser APIs and third-party APIs
- the key difference between a library and a framework is "Inversion of Control". when calling a method from a library, the developer is in control. with a framework, the control is inverted: the framework calls the developer's code.
- common browser APIs:
	- APIs for manipulating documents (DOM API)
	- APIs that fetch data from the server (Fetch API)
	- APIs for drawing and manipulating graphics (Canvas, WebGL)
	- Audio and Video APIs (HTMLMediaElement, Web Audio API, WebRTC)
	- Device APIs (Geolocation API)
	- Client-side storage APIs (Web Storage API, IndexedDB API)
- common third-party APIs
	- Twitter API
	- Mapquest, Google Maps API
	- Facebook suite of APIs
	- Telegram APIs
	- Youtube, Pinterest, Twilio, Mastodon API
- play() and pause() methods being used to play and pause the track are not part of the Web Audio API; they are part of the HTMLMediaElement API, which is different but closely-related.

manipulating documents
- the important parts of a web browser: navigator, window, document.
- the DOM tree diagram can be created by using Ian Hickon's Live DOM viewer
- each entry in the tree is called a node. nodes are also referred to by their position in the tree relative to other nodes: root node, child node, descendant node, parent node, sibling nodes.

fetching data from the server
- so instead of a traditional model, many websites use JavaScript APIs to request data from the server and update the page content without a page load. so when the user search for a new product, the browser only requests the data which is needed to update the page -- the set of new books to display, for instance.
- the main API here is the Fetch API. this enables JavaScript running in a page to make an HTTP request to a servr to retrieve specific resources. when the server provides them, the JS can use the data to update the page. the data requested is often JSON, which is a good format for transferring structured data, but can also be HTML or just text.