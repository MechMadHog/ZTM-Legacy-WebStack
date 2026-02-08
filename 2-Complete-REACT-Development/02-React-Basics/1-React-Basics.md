# React Basics - Pre-Coding Setup

This section defines the environment, tooling, and expectations before writing any React code. The goal is to remove friction so focus stays on learning architecture and workflow.

---

## Learning goals

This course is about learning how to architect React applications, not just writing syntax.

Projects start small and expand in scope to reinforce:

* structure
* organization
* scalable thinking

These lessons are designed as **code-along exercises**, so active participation is expected.

---

## Core tooling

### Project tooling

* **Create React App**
  Used to scaffold a local React environment with sensible defaults.

* **GitHub Pages**
  Used to deploy finished projects for public viewing.

### Required comfort level

Before continuing, you should be comfortable with:

* basic terminal usage
* navigating files and running commands
* working inside VS Codium

The terminal is the primary interface for managing projects.

---

## Platform setup

### Environment

My setup is:

* Omarchy (Linux environment)
* VS Codium as the editor

This environment already includes most development tools.

### Terminal workflow

The terminal is used to:

* navigate project folders
* run development commands
* manage dependencies
* modify project structure

Git functionality is already available through the system and editor integration.

---

## Node ecosystem

Modern React workflows depend on Node-based tooling.

* **nvm (Node Version Manager)**
  Installs and manages Node versions safely.

* **Node.js**
  Provides runtime and development tooling.

* **npm**
  Default package manager included with Node.

* **Yarn**
  Alternative package manager used throughout the course.

### npm vs Yarn reference

Both tools accomplish the same tasks.

| Task                 | npm                              | Yarn                      |
| -------------------- | -------------------------------- | ------------------------- |
| Install dependencies | `npm install`                    | `yarn`                    |
| Add dependency       | `npm install package --save`     | `yarn add package`        |
| Add dev dependency   | `npm install package --save-dev` | `yarn add package --dev`  |
| Remove dependency    | `npm uninstall package --save`   | `yarn remove package`     |
| Upgrade package      | `npm update --save`              | `yarn upgrade`            |
| Global install       | `npm install -g package`         | `yarn global add package` |

These commands will be practiced during the course.

---

## Editor configuration

The instructor demonstrates a themed VS Code setup. Functionality matters more than matching visuals.

### Optional font setup

The course uses **Operator Mono Lig** with ligatures enabled. This is aesthetic only.

If desired:

Editor → Font Family

```
Operator Mono Lig, Menlo, Monaco, monospace
```

Editor → Font Ligatures

```
enabled
```

Any readable cyberpunk-style font or theme can be substituted.

### Recommended productivity extensions

* ESLint
* Prettier
* Path Intellisense
* Auto Close Tag

These improve workflow consistency.

### Optional development extensions

* React snippets
* GraphQL syntax highlighting
* Markdown tools
* Styled-components highlighting

### Visual extensions (optional)

* Snazzy Operator
* color themes
* icon packs

Use whatever theme supports readability and comfort.

Restart the editor after installing fonts or extensions if changes do not appear.

### Editor philosophy

Prioritize:

* readability
* speed
* comfort
* consistency

Visual styling is secondary to workflow.

---

## Explorer display adjustment

Recent updates compress folders with single children into stacked paths. This can make tutorial structures harder to follow.

### Restore classic folder view

1. Open **Settings** (`Ctrl + ,`)
2. Navigate to:

```
Features → Explorer
```

3. Disable **Compact Folders**

Folders will display individually again.

This change only affects appearance, not file behavior.

---

## Reference resources

* Node.js
  [https://nodejs.org/en/](https://nodejs.org/en/)

* Sandbox environment
  [https://codesandbox.io/s/new](https://codesandbox.io/s/new)

* React documentation
  [https://react.dev/learn](https://react.dev/learn)

---

## Purpose of this setup

This environment supports:

* local React development
* dependency management
* scalable workflow habits

Everything above establishes a stable foundation before coding begins.
