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

#### Import Java classes as data types

Use the `dmn-cli fetch-types <JAVA_PROJECT_PATH>` command to generate a **types.dmn** model with all types from a Java project.

```bash
dmn-cli fetch-types ~/Mortgages
```

#### Import JSON objects as data types

Use the `dmn-cli fetch-types <JSON_FILE_PATH>` command to generate a **types.dmn** model with all types defined into the JSON object.

```bash
dmn-cli fetch-types data-types.json
```

Here's an example of a JSON object with some data types:

```
[
  {
    "name": "tPerson",
    "children": [
      { "name": "id", "type": "tUUID" },
      { "name": "name", "type": "string" },
      { "name": "age", "type": "string" }
    ]
  },
  {
    "name": "tUUID",
    "children": [
      { "name": "prefix", "type": "string" },
      { "name": "hash", "type": "string" }
    ]
  }
]
```

#### Preview the model

Use the `dmn-cli preview <DMN_MODEL_PATH>` command to generate a **diagram.png** file and automatically open this diagram preview.

```bash
dmn-cli preview ~/my-model.dmn
```

#### Inspect elements

Use the `dmn-cli inspect <DMN_MODEL_PATH>` command to list the main DMN model elements and version.

```bash
dmn-cli inspect ~/my-model.dmn
```
