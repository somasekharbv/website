---
id: version-6.x-babel-plugin-transform-es3-member-expression-literals
title: babel-plugin-transform-es3-member-expression-literals
sidebar_label: transform-es3-member-expression-literals
original_id: babel-plugin-transform-es3-member-expression-literals
---

## Example

**In**

```javascript
foo.catch;
```

**Out**

```javascript
foo["catch"];
```

## Installation

```sh
npm install --save-dev babel-plugin-transform-es3-member-expression-literals
```

## Usage

### Via `.babelrc` (Recommended)

**.babelrc**

```json
{
  "plugins": ["transform-es3-member-expression-literals"]
}
```

### Via CLI

```sh
babel --plugins transform-es3-member-expression-literals script.js
```

### Via Node API

```javascript
require("babel-core").transform("code", {
  plugins: ["transform-es3-member-expression-literals"]
});
```

