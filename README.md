Reacto is a set of CLI commands to maintain react.js apps and components based on [specific structure](#component-structure) we use in ottofeller.com. It is mostly a wrapper around https://github.com/audreyr/cookiecutter with some additional features like adding additional parts (like actions or routes) into existing component.

The main reason why it is not an npm, but pypi package is that there is no cookiecutter port for node.js with non-CLI API.

## Component structure
*To be edited*

## Installation
Simply install pypi package:
```shell
pip install reacto
```

CLI script will deploy into some of your `bin/` directories, make sure it is listed in `$PATH`.

## Available commands and options

### `start_app [options] <app path>`
*Not yet available*

### `start_component [options] <component path>`
Start new component. You can pass absolute/relative path or just compoentn name, in which case component will be created in current directory.

#### `--actions`
If passed `<component path>/actions.js` file created.

#### `--no-flow`
*To be edited*

#### `--reducers`
If passed `<component path>/reducers.js` file created.

#### `--routes`
If passed React Router 4 will be applied to `idex.js`.

#### `--route-path`
Path specified on root component of routes tree, which is `routes.js:<Route />`.

### `class2function [options] <component path>`
*Not yet available*

### `function2class [options] <component path>`
*Not yet available*
