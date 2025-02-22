---
date: 2021-12-17
title: Components of a successful design system
# shortDescription: Some reasons why I choose React Testing Library over Enzyme for testing React components
category: template
# tags: [react, hooks]
# hero: ./blue-anchor-on-wall.jpg
# heroAlt: Blue anchor stenciled on the wall
# heroCredit: 'Photo by [milan degraeve](https://unsplash.com/@milandegraeve)'
published: false
---

- Talking about internal-only
  - Public ones have to be anything & everything to everyone
- Non-obvious things
  - Design system checklist: https://designsystemchecklist.com/

1. Design team **must** drive the process and be bought-in otherwise don't bother (see previous post)
1. Box & Text components

- Everyone always starts w/ button
- Spacing helpers (in your units)
- Width helpers
- Text has typography settings: styles, sizes, weights
- Can be set to any tag

1. Icon components

- Individual component per svg, no iconography lookup
- Should be resizable and colorizable (use paths)

1. Disallow style & class names on every other component (radical idea)
1. Provide more flexibility than what's designed
1. Provide UI escape hatches (i.e. render props)
1. Stack & Inline layout components
1. Base components for buttons, toggles, single select, multi-select (on demand of course)

- Share logic
- Bake in accessibility

1. Section for "prototypes"

- A place for you or other teams to experiment w/ components that aren't "blessed"

Keep learning my friends. 🤓
