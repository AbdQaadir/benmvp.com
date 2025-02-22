---
date: 2021-12-17
title: React render props in TypeScript
# shortDescription: Some reasons why I choose React Testing Library over Enzyme for testing React components
category: template
# tags: [react, hooks]
# hero: ./blue-anchor-on-wall.jpg
# heroAlt: Blue anchor stenciled on the wall
# heroCredit: 'Photo by [milan degraeve](https://unsplash.com/@milandegraeve)'
published: false
---

One of my biggest pet peeves with React [`prop-types`](https://www.npmjs.com/package/prop-types) is the weak prop validation for function props.

```js
Example.propTypes = {
  onClick: PropTypes.func,
  onChange: PropTypes.func,
  onSelect: PropTypes.func,
}
```

Are any parameter passed to `onClick`? How many arguments are passed to `onChange`? Will I get the `event` object with `onSelect`? We have to rely on really good docs (😂) or looking at the source code to know what sort of function we can pass to function props.

And it's even more confusing with "inversion of control" function props that are expected to return a value. This is when the child component provides some internal state to the parent component by calling a function prop, and uses the return value to render UI, maintain more additional state, etc.

One example of an "inversion of control" function prop is the [render prop](https://ui.dev/react-render-props/). The component defines a function prop, typically called `render` or `children`, passes internal state to the function, and renders the UI returned by the function. It allows the component abstract or consolidate stateful logic, but offload the UI to the caller.

```js

```

TODO:

- Update the TS + React prop types posts w/ links to this and other related posts

Keep learning my friends. 🤓
