## React Concepts

### The birth of React.js (2013)

Before modern front-end frameworks, the browser stack was simple:

* **HTML** → page structure
* **CSS** → presentation and layout
* **JavaScript** → interactivity

Early web applications revolved around forms. Users submitted data to a server, the server processed it, and a new page was returned. This request-response model defined how most sites behaved.

A major challenge was browser inconsistency. Different browsers interpreted JavaScript differently, forcing developers to write compatibility workarounds.

### The rise of libraries and structure

To address cross-browser issues, **jQuery** provided a consistent way to interact with the DOM (Document Object Model). It simplified event handling, animations, and element manipulation, allowing developers to focus more on behavior instead of compatibility fixes.

As applications grew, JavaScript codebases became harder to manage. Frameworks such as **Backbone.js** introduced structure and organization, helping developers separate concerns and control increasing complexity.

This evolution contributed to the rise of **single page applications (SPAs)** powered by AJAX. Instead of reloading entire pages, applications dynamically updated content, creating smoother user experiences.

### Framework standardization

In 2010, Google released **AngularJS**, which quickly became a major front-end framework. It promoted structured architecture using an MVC (Model View Controller) pattern, organizing code by responsibility and encouraging large-scale application design.

### Why React emerged

As front-end systems continued to grow in complexity, Facebook engineers faced recurring architectural challenges across large teams. React.js was created to improve consistency, maintainability, and predictable UI behavior.

Its design emphasized component architecture and clear data flow, allowing teams to scale applications without losing structural clarity.

React represented a shift from page-driven development toward composable UI systems built for modern, interactive applications.

---

## 1. Don’t touch the DOM… I’ll handle it.

React changes how developers think about UI updates.

**Imperative programming** means directly manipulating individual parts of the interface:

“If this happens, change that element.”

As applications grow, this approach can create tightly coupled logic and DOM bottlenecks.

**Declarative programming** focuses on describing what the interface should look like based on current data.

In React, **state** represents the application’s data. The UI is derived from that state. When state changes, React determines what must update and applies those changes efficiently.

Instead of manually managing DOM operations, developers define intent and React handles the implementation.

---

## 2. Building websites like Lego blocks

### Component architecture

React applications are built from **reusable components**. Each component represents a focused piece of UI logic and presentation.

Components can contain other components to form complex layouts, similar to assembling modular building blocks. This promotes separation of concerns and makes large interfaces easier to reason about.

Libraries such as React Bootstrap or Blueprint.js provide prebuilt component systems that follow this model.

React Developer Tools allow developers to inspect component hierarchies, state, and props directly in the browser.

Under the hood, components ultimately render standard HTML elements organized through JavaScript logic.

---

## 3. Unidirectional data flow

React uses **JSX** to describe UI structure in a readable, component-focused syntax.

Internally, React generates a **virtual DOM**, a lightweight JavaScript representation of the UI. This acts as a blueprint for updating the real DOM efficiently.

When application data changes:

1. State is updated
2. React recalculates the UI representation
3. Only the required DOM changes are applied

This process enforces **unidirectional data flow**:

State → Components → UI

User interactions trigger events, events update state, and state drives UI changes. Because updates move in a predictable direction, applications are easier to debug, scale, and maintain.

These constraints reduce unintended side effects and keep rendering behavior consistent.

---

## 4. React is a UI library. The rest is up to you.

React focuses on one responsibility: building user interfaces. It does not enforce a specific technology stack, backend, or application architecture.

Because React is only concerned with UI logic, it can be adapted to many environments beyond the browser.

React Native applies the same component model to build iOS and Android applications.

React 360 extends the model into immersive and VR environments.

Electron combined with React Desktop allows developers to build desktop applications for Windows, macOS, and Linux using familiar web technologies.

React Blessed brings the component approach to terminal interfaces, enabling UI-driven command line tools.

This flexibility means React is effectively cross-platform. The same architectural principles can be reused regardless of where the interface runs.

### Core libraries

When building React applications for the web, two libraries are typically imported:

1. **React**
   The core library responsible for components, state management, and UI logic.

2. **React DOM**
   The layer that connects React to the browser by rendering components into the DOM.

Separating core logic from rendering allows React to target multiple platforms while keeping the development model consistent.

### Resources

* [https://reactdesktop.js.org/](https://reactdesktop.js.org/)
* [https://github.com/Yomguithereal/react-blessed](https://github.com/Yomguithereal/react-blessed)
* [https://facebook.github.io/react-360/](https://facebook.github.io/react-360/)

---

## How to be a great React developer

React is a **declarative** paradigm. It uses application **state** to drive UI behavior through **components** built with **JSX**. Those components receive **props**, and together they produce a JavaScript representation of the interface known as the **virtual DOM**. React uses this representation to efficiently update the real DOM.

A strong React developer understands how these pieces work together and can make deliberate architectural decisions.

### 1. Decide on components

Components define the structure of the application.

A good developer knows how to:

* Break UI into logical, reusable pieces
* Avoid components that are too large or too fragmented
* Separate concerns clearly

The goal is readable, maintainable structure. Components should have a focused responsibility and be easy to reason about.

### 2. Decide where state lives

State controls behavior and rendering.

A strong React developer considers:

* Which component owns the data
* Whether state should be shared or isolated
* How state flows through the component tree

State placement affects clarity, maintainability, and performance. Poor placement leads to unnecessary complexity or re-rendering.

### 3. Understand what changes when state changes

State updates trigger re-renders.

A developer should understand:

* Which components will re-render
* How changes propagate through the tree
* The performance implications of updates

Not every change should cause broad re-rendering. Predictable updates lead to smoother behavior and better user experience.

A great React developer is not just writing components. They are designing how data flows, how structure scales, and how updates affect the application as a whole.
