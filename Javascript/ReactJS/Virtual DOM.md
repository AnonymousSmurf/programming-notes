 # VDOM (Virtual DOM)
 
 The virtual DOM **(VDOM)** is a programming concept where an ideal, or “virtual”, representation of a UI is kept in memory and synced with the “real” DOM by a library such as ReactDOM.
 
 This approach enables the declarative API of React: You tell React what state you want the UI to be in, and it makes sure the DOM matches that state. This abstracts out the attribute manipulation, event handling, and manual DOM updating that you would otherwise have to use to build your app.

## How does React use the virtual DOM?

React uses virtual DOM to enhance its performance. It uses **the observable to detect state and prop changes**. React uses an efficient diff algorithm to compare the versions of virtual DOM. It then makes sure that batched updates are sent to the real DOM for repainting or re-rendering of the UI.
 
 #REACT