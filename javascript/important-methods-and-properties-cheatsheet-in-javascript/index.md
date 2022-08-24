Hello Everyone,

Here is the list of important methods and properties in JavaScript.
in this tutorial we are going to cover the following topics:

1. DOM Node Properties
2. DOM Node Methods
3. DOM Element Methods
4. Window Properties
5. Window Methods
6. Screen Properties
7. JavaScript Mouse Events
8. JavaScript Keyboard Events
9. JavaScript Frame Events
10. JavaScript Form Events
11. JavaScript Drag Events
12. JavaScript Clipboard Events
13. JavaScript Media Events
14. JavaScript Animation Events
15. JavaScript Other Events
16. Errors
17. Error Name Values
18. Quantifiers

# **DOM Node Properties**

- `attributes` — Returns a live collection of all attributes registered to an element
- `baseURI` — Provides the absolute base URL of an HTML element
- `childNodes` — Gives a collection of an element’s child nodes
- `firstChild` — Returns the first child node of an element
- `lastChild` — The last child node of an element
- `nextSibling` — Gives you the next node at the same node tree level
- `nodeName` —Returns the name of a node
- `nodeType` — Returns the type of a node
- `nodeValue` — Sets or returns the value of a node
- `ownerDocument` — The top-level document object for this node
- `parentNode` — Returns the parent node of an element
- `previousSibling` — Returns the node immediately preceding the current one
- `textContent` — Sets or returns the textual content of a node and its descendants

# **DOM Node Methods**

- `appendChild()` — Adds a new child node to an element as the last child node
- `cloneNode()` — Clones an HTML element
- `compareDocumentPosition()` — Compares the document position of two elements
- `getFeature()` — Returns an object which implements the APIs of a specified feature
- `hasAttributes()` — Returns true if an element has any attributes, otherwise false
- `hasChildNodes()` — Returns true if an element has any child nodes, otherwise false
- `insertBefore()` — Inserts a new child node before a specified, existing child node
- `isDefaultNamespace()` — Returns true if a specified namespaceURI is the default, otherwise false
- `isEqualNode()` — Checks if two elements are equal
- `isSameNode()` — Checks if two elements are the same node
- `isSupported()` — Returns true if a specified feature is supported on the element
- `lookupNamespaceURI()` — Returns the namespace URI associated with a given node
- `lookupPrefix()` — Returns a DOMString containing the prefix for a given namespace URI if present
- `normalize()` — Joins adjacent text nodes and removes empty text nodes in an element
- `removeChild()` — Removes a child node from an element
- `replaceChild()` — Replaces a child node in an element

# **DOM Element Methods**

- `getAttribute()` — Returns the specified attribute value of an element node
- `getAttributeNS()` — Returns string value of the attribute with the specified namespace and name
- `getAttributeNode()` — Gets the specified attribute node
- `getAttributeNodeNS()` — Returns the attribute node for the attribute with the given namespace and name
- `getElementsByTagName()` — Provides a collection of all child elements with the specified tag name
- `getElementsByTagNameNS()` — Returns a live HTMLCollection of elements with a certain tag name belonging to the given namespace
- `hasAttribute()` — Returns true if an element has any attributes, otherwise false
- `hasAttributeNS()` — Provides a true/false value indicating whether the current element in a given namespace has the specified attribute
- `removeAttribute()` — Removes a specified attribute from an element
- `removeAttributeNS()` — Removes the specified attribute from an element within a certain namespace
- `removeAttributeNode()` — Takes away a specified attribute node and returns the removed node
- `setAttribute()` — Sets or changes the specified attribute to a specified value
- `setAttributeNS()` — Adds a new attribute or changes the value of an attribute with the given namespace and name
- `setAttributeNode()` — Sets or changes the specified attribute node
- `setAttributeNodeNS()` — Adds a new namespaced attribute node to an element

# **Window Properties**

- `closed` — Checks whether a window has been closed or not and returns true or false
- `defaultStatus` — Sets or returns the default text in the status bar of a window
- `document` — Returns the document object for the window
- `frames` — Returns all `<iframe>` elements in the current window
- `history` — Provides the History object for the window
- `innerHeight` — The inner height of a window’s content area
- `innerWidth` — The inner width of the content area
- `length` — Find out the number of `<iframe>` elements in the window
- `location` — Returns the location object for the window
- `name` — Sets or returns the name of a window
- `navigator` — Returns the Navigator object for the window
- `opener` — Returns a reference to the window that created the window
- `outerHeight` — The outer height of a window, including toolbars/scrollbars
- `outerWidth` — The outer width of a window, including toolbars/scrollbars
- `pageXOffset` — Number of pixels the current document has been scrolled horizontally
- `pageYOffset` — Number of pixels the document has been scrolled vertically
- `parent` — The parent window of the current window
- `screen` — Returns the Screen object for the window
- `screenLeft` — The horizontal coordinate of the window (relative to the screen)
- `screenTop` — The vertical coordinate of the window
- `screenX` — Same as `screenLeft` but needed for some browsers
- `screenY` — Same as `screenTop` but needed for some browsers
- `self` — Returns the current window
- `status` — Sets or returns the text in the status bar of a window
- `top` — Returns the topmost browser window

# **Window Methods**

- `alert()` — Displays an alert box with a message and an OK button
- `blur()` — Removes focus from the current window
- `clearInterval()` — Clears a timer set with `setInterval()`
- `clearTimeout()` — Clears a timer set with `setTimeout()`
- `close()` — Closes the current window
- `confirm()` — Displays a dialogue box with a message and an *OK* and *Cancel* button
- `focus()` — Sets focus to the current window
- `moveBy()` — Moves a window relative to its current position
- `moveTo()` — Moves a window to a specified position
- `open()` — Opens a new browser window
- `print()` — Prints the content of the current window
- `prompt()` — Displays a dialogue box that prompts the visitor for input
- `resizeBy()` — Resizes the window by the specified number of pixels
- `resizeTo()` — Resizes the window to a specified width and height
- `scrollBy()` — Scrolls the document by a specified number of pixels
- `scrollTo()` — Scrolls the document to specified coordinates
- `setInterval()` — Calls a function or evaluates an expression at specified intervals
- `setTimeout()` — Calls a function or evaluates an expression after a specified interval
- `stop()` — Stops the window from loading

# **Screen Properties**

- `availHeight` — Returns the height of the screen (excluding the Windows Taskbar)
- `availWidth` — Returns the width of the screen (excluding the Windows Taskbar)
- `colorDepth` — Returns the bit depth of the color palette for displaying images
- `height` — The total height of the screen
- `pixelDepth` — The color resolution of the screen in bits per pixel
- `width` — The total width of the screen

# **JavaScript Events**

Events are things that can happen to HTML elements and are performed by the user. The programming language can listen for these events and trigger actions in the code. No JavaScript cheat sheet would be complete without them.

# **Mouse**

- `onclick` — The event occurs when the user clicks on an element
- `oncontextmenu` — User right-clicks on an element to open a context menu
- `ondblclick` — The user double-clicks on an element
- `onmousedown` — User presses a mouse button over an element
- `onmouseenter` — The pointer moves onto an element
- `onmouseleave` — Pointer moves out of an element
- `onmousemove` — The pointer is moving while it is over an element
- `onmouseover` — When the pointer is moved onto an element or one of its children
- `onmouseout` — User moves the mouse pointer out of an element or one of its children
- `onmouseup` — The user releases a mouse button while over an element

# **Keyboard**

- `onkeydown` — When the user is pressing a key down
- `onkeypress` — The moment the user starts pressing a key
- `onkeyup` — The user releases a key

# **Frame**

- `onabort` — The loading of a media is aborted
- `onbeforeunload` — Event occurs before the document is about to be unloaded
- `onerror` — An error occurs while loading an external file
- `onhashchange` — There have been changes to the anchor part of a URL
- `onload` — When an object has loaded
- `onpagehide` — The user navigates away from a webpage
- `onpageshow` — When the user navigates to a webpage
- `onresize` — The document view is resized
- `onscroll` — An element’s scrollbar is being scrolled
- `onunload` — Event occurs when a page has unloaded

# **Form**

- `onblur` — When an element loses focus
- `onchange` — The content of a form element changes (for `<input>`, `<select>` and `<textarea>`)
- `onfocus` — An element gets focus
- `onfocusin` — When an element is about to get focus
- `onfocusout` — The element is about to lose focus
- `oninput` — User input on an element
- `oninvalid` — An element is invalid
- `onreset` — A form is reset
- `onsearch` — The user writes something in a search field (for `<input="search">`)
- `onselect` — The user selects some text (for `<input>` and `<textarea>`)
- `onsubmit` — A form is submitted

# **Drag**

- `ondrag` — An element is dragged
- `ondragend` — The user has finished dragging the element
- `ondragenter` — The dragged element enters a drop target
- `ondragleave` — A dragged element leaves the drop target
- `ondragover` — The dragged element is on top of the drop target
- `ondragstart` — User starts to drag an element
- `ondrop` — Dragged element is dropped on the drop target

# **Clipboard**

- `oncopy` — User copies the content of an element
- `oncut` — The user cuts an element’s content
- `onpaste` — A user pastes the content in an element

# **Media**

- `onabort` — Media loading is aborted
- `oncanplay` — The browser can start playing media (e.g. a file has buffered enough)
- `oncanplaythrough` — The browser can play through media without stopping
- `ondurationchange` — The duration of the media changes
- `onended` — The media has reached its end
- `onerror` — Happens when an error occurs while loading an external file
- `onloadeddata` — Media data is loaded
- `onloadedmetadata` — Metadata (like dimensions and duration) are loaded
- `onloadstart` — The browser starts looking for specified media
- `onpause` — Media is paused either by the user or automatically
- `onplay` — The media has been started or is no longer paused
- `onplaying` — Media is playing after having been paused or stopped for buffering
- `onprogress` — The browser is in the process of downloading the media
- `onratechange` — The playing speed of the media changes
- `onseeked` — User is finished moving/skipping to a new position in the media
- `onseeking` — The user starts moving/skipping
- `onstalled` — The browser is trying to load the media but it is not available
- `onsuspend` — The browser is intentionally not loading media
- `ontimeupdate` — The playing position has changed (e.g. because of fast forward)
- `onvolumechange` — Media volume has changed (including mute)
- `onwaiting` — Media paused but expected to resume (for example, buffering)

# **Animation**

- `animationend` — A CSS animation is complete
- `animationiteration` — CSS animation is repeated
- `animationstart` — CSS animation has started

# **Other**

- `transitionend` — Fired when a CSS transition has completed
- `onmessage` — A message is received through the event source
- `onoffline` — The browser starts to work offline
- `ononline` — The browser starts to work online
- `onpopstate` — When the window’s history changes
- `onshow` — A `<menu>` element is shown as a context menu
- `onstorage` — A Web Storage area is updated
- `ontoggle` — The user opens or closes the `<details>` element
- `onwheel` — Mouse wheel rolls up or down over an element
- `ontouchcancel` — Screen-touch is interrupted
- `ontouchend` — User’s finger is removed from a touch-screen
- `ontouchmove` — A finger is dragged across the screen
- `ontouchstart` — A finger is placed on the touch-screen

# **Errors**

When working with JavaScript, different errors can occur. There are several ways of handling them:

- `try` — Lets you define a block of code to test for errors
- `catch` — Set up a block of code to execute in case of an error
- `throw` — Create custom error messages instead of the standard JavaScript errors
- `finally` — Lets you execute code, after try and catch, regardless of the result

# **Error Name Values**

JavaScript also has a built-in error object. It has two properties:

- `name` — Sets or returns the error name
- `message` — Sets or returns an error message in a string from

The error property can return six different values as its name:

- `EvalError` — An error has occurred in the `eval()` function
- `RangeError` — A number is “out of range”
- `ReferenceError` — An illegal reference has occurred
- `SyntaxError` — A syntax error has occurred
- `TypeError` — A type error has occurred
- `URIError` — An `encodeURI()` error has occurred

# **Quantifiers**

- `n+` — Matches any string that contains at least one n
- `n*` — Any string that contains zero or more occurrences of n
- `n?` — A string that contains zero or one occurrence of n
- `n{X}` — String that contains a sequence of X n’s
- `n{X,Y}` — Strings that contain a sequence of X to Y n’s
- `n{X,}` — Matches any string that contains a sequence of at least X n’s
- `n$` — Any string with n at the end of it
- `^n` — String with n at the beginning of it
- `?=n` — Any string that is followed by a specific string n
- `?!n` — String that is not followed by a specific string ni

If this is helpful for you, then let us know in the comment.

Thanks,\
CapsCode
