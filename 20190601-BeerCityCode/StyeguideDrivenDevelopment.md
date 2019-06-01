# TDD Designer Style - Styleguide Driven Development by Matthew LaForest

## Misc

TDD has been difficult to apply to UI/UX, as traditionally testing techniques try to describe the UI from a programatic point of view; just because a UI element has the right class doesn't mean it looks good.

Styleguides help establish a common "language" for the application, and are adapted from the print world.

Showcased Storybook: an applcation used to build a living styleguide. Components (a.k.a. atoms) can be developed within any of the major front-end frameworks and combined/built out into larger sections (blocks, templates, features). This allows components to be viewied within context and visually see how everything fits together instead of just viewing components in isolation.

Living styleguides can help an application be built interatively, as a system is in place to check eveyrthing still looks right through refactoring.

Tools like Percy are available to tie visuals checks into the CI process.

Try to keep low level components as close to basic HTML elements as possible; essentially just use them as style wrappers, and not give them extra properties/interactions.
