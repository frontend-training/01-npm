# NPM

---

# What is NPM?

It is the default package manager for the JavaScript runtime environment Node.js. It consists of a command line client, also called npm, and an online database of public and paid-for private packages, called the npm registry.

---

# package.json

```json
{
  "name": "cowgreet",
  "version": "1.0.0",
  "description": "A legen dairy interface for communicating with cattle",
  "main": "index.js",
  "scripts": {
    "moo": "node index.js"
  },
  "author": "Bobby Nae",
  "license": "ISC",
  "dependencies": {}
}
```

---

# How to Install a Package?

- Find it by name.
- Install it.
  - Globally: `npm install -g typescript`
  - Locally: `npm install --save cowsay`
  - For dev only: `npm install --save-dev jest`

---

# The package-lock.json

 It describes the exact tree that was generated, such that subsequent installs are able to generate identical trees, regardless of intermediate dependency updates.

 ---

## Tips
- commit it.
- remove it to refresh floating dependencies.

---

# Semver Ranges

> X-Ranges 1.2.x 1.X 1.2.*

Any of X, x, or * may be used to “stand in” for one of the numeric values in the

---

# Semver Ranges

> ~1.2.3 ~1.2 ~1

Allows patch-level changes if a minor version is specified on the comparator.
Allows minor-level changes if not.

---

# Semver Ranges

> ^1.2.3 ^0.2.5 ^0.0.4§

Allows changes that do not modify the left-most non-zero digit in the [major, minor, patch] tuple.

In other words, this allows patch and minor updates for versions 1.0.0 and above,
patch updates for versions 0.X >=0.1.0,
and no updates for versions 0.0.X.

---

# NPM vs Yarn

Yarn is Facebook's alternative to npm as a dependency management tool.

- Better ui.
- Caching.
- Different flavor.
- Pretty much the same.

Still, worth checking out. https://yarnpkg.com/

---

# NPM for Tooling

Is mostly used for:
- Building your project.
- Building assets.
  - scss -> css
  - png -> base64
- Transpiling your TypeScript to JavaScript.
- Running your project in development mode.
- Linting.
- Different pipelines.

---

# NPM for Tooling

Can be used for:
- Deploying.
- Serving your app in the real world.
- Almost anything, tbh.

---

# FIN
