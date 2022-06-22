oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @vikadadta/transformer
$ @vikadadta/transformer COMMAND
running command...
$ @vikadadta/transformer (--version)
@vikadadta/transformer/0.0.0 linux-x64 node-v16.15.1
$ @vikadadta/transformer --help [COMMAND]
USAGE
  $ @vikadadta/transformer COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`@vikadadta/transformer hello PERSON`](#vikadadtatransformer-hello-person)
* [`@vikadadta/transformer hello world`](#vikadadtatransformer-hello-world)
* [`@vikadadta/transformer help [COMMAND]`](#vikadadtatransformer-help-command)
* [`@vikadadta/transformer plugins`](#vikadadtatransformer-plugins)
* [`@vikadadta/transformer plugins:install PLUGIN...`](#vikadadtatransformer-pluginsinstall-plugin)
* [`@vikadadta/transformer plugins:inspect PLUGIN...`](#vikadadtatransformer-pluginsinspect-plugin)
* [`@vikadadta/transformer plugins:install PLUGIN...`](#vikadadtatransformer-pluginsinstall-plugin-1)
* [`@vikadadta/transformer plugins:link PLUGIN`](#vikadadtatransformer-pluginslink-plugin)
* [`@vikadadta/transformer plugins:uninstall PLUGIN...`](#vikadadtatransformer-pluginsuninstall-plugin)
* [`@vikadadta/transformer plugins:uninstall PLUGIN...`](#vikadadtatransformer-pluginsuninstall-plugin-1)
* [`@vikadadta/transformer plugins:uninstall PLUGIN...`](#vikadadtatransformer-pluginsuninstall-plugin-2)
* [`@vikadadta/transformer plugins update`](#vikadadtatransformer-plugins-update)

## `@vikadadta/transformer hello PERSON`

Say hello

```
USAGE
  $ @vikadadta/transformer hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Whom is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/vikadata/datasheet-transformer/datasheet-transformer/blob/v0.0.0/dist/commands/hello/index.ts)_

## `@vikadadta/transformer hello world`

Say hello world

```
USAGE
  $ @vikadadta/transformer hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ oex hello world
  hello world! (./src/commands/hello/world.ts)
```

## `@vikadadta/transformer help [COMMAND]`

Display help for @vikadadta/transformer.

```
USAGE
  $ @vikadadta/transformer help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for @vikadadta/transformer.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `@vikadadta/transformer plugins`

List installed plugins.

```
USAGE
  $ @vikadadta/transformer plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ @vikadadta/transformer plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `@vikadadta/transformer plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ @vikadadta/transformer plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ @vikadadta/transformer plugins add

EXAMPLES
  $ @vikadadta/transformer plugins:install myplugin 

  $ @vikadadta/transformer plugins:install https://github.com/someuser/someplugin

  $ @vikadadta/transformer plugins:install someuser/someplugin
```

## `@vikadadta/transformer plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ @vikadadta/transformer plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ @vikadadta/transformer plugins:inspect myplugin
```

## `@vikadadta/transformer plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ @vikadadta/transformer plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ @vikadadta/transformer plugins add

EXAMPLES
  $ @vikadadta/transformer plugins:install myplugin 

  $ @vikadadta/transformer plugins:install https://github.com/someuser/someplugin

  $ @vikadadta/transformer plugins:install someuser/someplugin
```

## `@vikadadta/transformer plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ @vikadadta/transformer plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ @vikadadta/transformer plugins:link myplugin
```

## `@vikadadta/transformer plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ @vikadadta/transformer plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ @vikadadta/transformer plugins unlink
  $ @vikadadta/transformer plugins remove
```

## `@vikadadta/transformer plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ @vikadadta/transformer plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ @vikadadta/transformer plugins unlink
  $ @vikadadta/transformer plugins remove
```

## `@vikadadta/transformer plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ @vikadadta/transformer plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ @vikadadta/transformer plugins unlink
  $ @vikadadta/transformer plugins remove
```

## `@vikadadta/transformer plugins update`

Update installed plugins.

```
USAGE
  $ @vikadadta/transformer plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
