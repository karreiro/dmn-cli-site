---
layout: default
---

## Installation

Make sure you have [Node.js and the npm package manager](https://nodejs.org/en/download), and then install **dmn-cli**:

```bash
npm i -g dmn-cli
```

Check if the **dmn-cli** is correctly installed by executing:

```bash
dmn-cli --version
```

## Usage

#### Preview the model

Use the `preview` command to generate a **diagram.png** file and automatically open this diagram preview.

```
dmn-cli preview ~/my-model.dmn
```

#### Inspect elements

Use the `inspect` command to list the main DMN model elements and version.

```
dmn-cli inspect ~/my-model.dmn
```
