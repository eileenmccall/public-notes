- Limitations of CSS-only transitions/animations
    - Can wind up with lots of not displayed elements cluttering up the DOM
    - If an element is removed (as via a ternary) no outro animations can play because it is instantly removed from the DOM
        - For performance reasons, React doesn't wait to see if any elements need to render animations before removing them
- [react-transition-group](https://github.com/reactjs/react-transition-group)
    - Allows you to smoothly animate elements when they are added to and removed from the DOM
    - Can use `<Transition>` component to manage transition state manually
        - https://reactcommunity.org/react-transition-group/transition
    - Can use `<CSSTransition>` to simply add CSS classes to the wrapped element automatically
        - https://reactcommunity.org/react-transition-group/css-transition
    - Can use `<TransitionGroup>` to manage transitions for lists of items
        - https://reactcommunity.org/react-transition-group/transition-group
        - Wraps lists of `<Transition>` and `<CSSTransition>` components
        - Automatically manages their `in` prop whenever an item is added or removed from the list
    - Can cause animation timing issues if the actual CSS animation and the `timeout` prop passed to the `<Transition>` or `<CSSTransiton>` component are not the same
        - `timeout` just refers to how long the component will wait between state transitons
        - You can give the `entering` transition and the `exiting` transition different durations by passing an object with `enter` and `exit` keys with durations in milliseconds
- [react-motion](https://github.com/chenglou/react-motion)
- [react-move](https://react-move.js.org/#/)
- [react-router-transition](https://github.com/maisano/react-router-transition)