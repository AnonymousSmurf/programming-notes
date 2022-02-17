# DOM (Document Object Model)
## What is a DOM?
When a web page is loaded, the browser creates a **D**ocument **O**bject **M**odel of the page. The **HTML DOM** model is constructed as a tree of **Objects**.

*Example DOM:*
![[dom-example.png]]

## What is it used for?
The Document Object Model (DOM) is an **application programming interface (API) for HTML and XML documents** in the shape of a tree branch with **Objects**. It defines the logical structure of documents and the way a document is accessed and manipulated.

## Core of the DOM
The `document` and `window` objects are the objects whose interfaces you generally use most often in DOM programming. In simple terms, the `window` object represents something like the browser, and the `document` object is the root of the document itself. `Element` inherits from the generic `Node` interface, and together these two interfaces provide many of the methods and properties you use on individual elements. These elements may also have specific interfaces for dealing with the kind of data those elements hold, as in the `table` object example in the previous section.

#JAVASCRIPT