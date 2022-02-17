# Hooks
Hooks are **functions that let you `hook into` React state and lifecycle features from function** components. Hooks don't work inside classes — they let you use React without classes. You can also create your own Hooks to reuse stateful behavior between different components.

## Types of hooks
### State Hook
useState is a Hook **that allows you to have state variables in functional components**. You pass the initial state to this function and it returns a variable with the current state value (not necessarily the initial state) and another function to update this value.

*example:*
```jsx
import React, { useState } from 'react';
function Example() {
  // Declare a new state variable, which we'll call "count"
  const [count, setCount] = useState(0);
  return (
    <div>
      <p>You clicked {count} times</p>
      <button onClick={() => setCount(count + 1)}>
        Click me
      </button>
    </div>
  );
}
```


#REACT