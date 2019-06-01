# Web Components & Design Systems by Dale Sande

It's a loaded defintion; different people will give different answers.

## Available Design Systems

A lot... (Alaska Airlines has one of there own, that the author contributes to: Orion Design System).

- Lightning Design System - SalesForce

Don't use an existing design system; use them to draw inspiration.

## Components

Not talking about specific framework (i.e. React) components; strive for system that's system-agnostic.

## Misc

A.k.a pattern libraries, or UI Toolkits

Has two parts: design and code.

Goal is to drive design consistency.

### Design

Involves tools like Sketch. Define typography, colors, rules on spacing, etc.

### Code (non Web-Components)

The HTML, CSS/SASS/LESS, and framework components that implements the design on the web.

Cause more problems than they solve. They're blueprints at best, not strict enforcements.

#### Failure Reasons

Copy/paste HTML will mutate, breaking the contract of the design system.

CSS naming conventions are doomed to fail, as they cannot be enforced. It's too difficult to keep in sync amongst multiple developers.

The same framework isn't used across all teams in all projects, and only has a finite lifetime. And they cannot solve the CSS problems. CSS in JS is only masking the issue. Anything that deviates from the standard will be difficult to maintain long-term. Frameworks typically become monolithic at some point.

### Web Components

Custom elements within the W3C spec.

Encapsulates CSS, JS, and UX. Nothing eternal comes in, and nothing bleeds out. Caveat: CSS variables pierce through the Shadow DOM.

Can be delivered as versioned packages. Keep things small and stateless.

Examples: [Microsoft Graph Toolkit](https://github.com/microsoftgraph/microsoft-graph-toolkit)

#### Browser Support

All modern browsers (Edge still WIP) have native support. Polyfills exists to hook support in (TODO: verify this is true with IE.)

#### Negatives

Have to re-define element attributes (e.g. `disabled` on a `button`). Accessibility can be a little funcky. Take a look at the progress of the Accessiblity Object Model.

#### Available Tools

[lit-element](https://github.com/Polymer/lit-element) base class for creating web components.
[Open WC](https://github.com/open-wc/open-wc)
(https://www.npmjs.com/package/wc-sass-render)
