
# ReactDOM
The `react-dom` package provides DOM-specific methods that can be used at the top level of your app and as an escape hatch to get outside of the React model if you need to. Most of your components should not need to use this module.

## Methods
### render()
```jsx
ReactDOM.render(element, container[, callback])
```
Render a React element into the DOM in the supplied `container` and return a `reference` to the component (or returns `null` for `stateless components`)

If the React element was previously rendered into `container`, this will perform an update on it and only mutate the DOM as necessary to reflect the latest React element.

If the optional callback is provided, it will be executed after the component is rendered or updated.

### hydrate()
```jsx
ReactDOM.hydrate(element, container[, callback])
```

Same as `render()`, but is used to hydrate a container whose HTML contents were rendered by `ReactDOMServer`. React will attempt to attach event listeners to the existing markup.

#REACT 