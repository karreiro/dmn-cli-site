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

Use the `dmn-cli fetch-types <java_project_path>` command to generate a **types.dmn** model with all types from a Java project.

```bash
dmn-cli fetch-types ~/Mortgages
```

#### Preview the model

Use the `dmn-cli preview <dmn_model_path>` command to generate a **diagram.png** file and automatically open this diagram preview.

```bash
dmn-cli preview ~/my-model.dmn
```

#### Inspect elements

Use the `dmn-cli inspect <dmn_model_path>` command to list the main DMN model elements and version.

```bash
dmn-cli inspect ~/my-model.dmn
```
