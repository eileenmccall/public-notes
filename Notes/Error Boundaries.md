- Custom error boundaries need to be class components
    - Need custom `static` method called `getDerivedStateFromError` which handles error
- To avoid using class components, you can use [react-error-boundary](https://github.com/bvaughn/react-error-boundary)
- Error boundary components can handle any errors thrown by their descendents
    - Errors are handled by the **nearest** boundary in the component tree, and do not bubble up to other boundaries
- Will render something else in place of its descendents in the event of an error (provided via `FallbackComponent` prop, or rendered manually within the error boundary if it's a custom implementation)
- Error boundaries only handle errors that occur within the React call stack.
    - **Includes:**
        - Render method
        - Functional component body
        - `useEffect` callback
    - **Excludes**:
        - Event handlers
        - Asynchronous callbacks in promise chains