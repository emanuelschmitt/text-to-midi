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
$ npm install -g text-to-midi
$ text-to-midi COMMAND
running command...
$ text-to-midi (--version)
text-to-midi/0.0.0 darwin-arm64 node-v16.13.0
$ text-to-midi --help [COMMAND]
USAGE
  $ text-to-midi COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`text-to-midi hello PERSON`](#text-to-midi-hello-person)
* [`text-to-midi hello world`](#text-to-midi-hello-world)
* [`text-to-midi help [COMMANDS]`](#text-to-midi-help-commands)
* [`text-to-midi plugins`](#text-to-midi-plugins)
* [`text-to-midi plugins:install PLUGIN...`](#text-to-midi-pluginsinstall-plugin)
* [`text-to-midi plugins:inspect PLUGIN...`](#text-to-midi-pluginsinspect-plugin)
* [`text-to-midi plugins:install PLUGIN...`](#text-to-midi-pluginsinstall-plugin-1)
* [`text-to-midi plugins:link PLUGIN`](#text-to-midi-pluginslink-plugin)
* [`text-to-midi plugins:uninstall PLUGIN...`](#text-to-midi-pluginsuninstall-plugin)
* [`text-to-midi plugins:uninstall PLUGIN...`](#text-to-midi-pluginsuninstall-plugin-1)
* [`text-to-midi plugins:uninstall PLUGIN...`](#text-to-midi-pluginsuninstall-plugin-2)
* [`text-to-midi plugins update`](#text-to-midi-plugins-update)

## `text-to-midi hello PERSON`

Say hello

```
USAGE
  $ text-to-midi hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/emanuelschmitt/text-to-midi/blob/v0.0.0/dist/commands/hello/index.ts)_

## `text-to-midi hello world`

Say hello world

```
USAGE
  $ text-to-midi hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ text-to-midi hello world
  hello world! (./src/commands/hello/world.ts)
```

## `text-to-midi help [COMMANDS]`

Display help for text-to-midi.

```
USAGE
  $ text-to-midi help [COMMANDS] [-n]

ARGUMENTS
  COMMANDS  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for text-to-midi.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.2.9/src/commands/help.ts)_

## `text-to-midi plugins`

List installed plugins.

```
USAGE
  $ text-to-midi plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ text-to-midi plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.4.4/src/commands/plugins/index.ts)_

## `text-to-midi plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ text-to-midi plugins:install PLUGIN...

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
  $ text-to-midi plugins add

EXAMPLES
  $ text-to-midi plugins:install myplugin 

  $ text-to-midi plugins:install https://github.com/someuser/someplugin

  $ text-to-midi plugins:install someuser/someplugin
```

## `text-to-midi plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ text-to-midi plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ text-to-midi plugins:inspect myplugin
```

## `text-to-midi plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ text-to-midi plugins:install PLUGIN...

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
  $ text-to-midi plugins add

EXAMPLES
  $ text-to-midi plugins:install myplugin 

  $ text-to-midi plugins:install https://github.com/someuser/someplugin

  $ text-to-midi plugins:install someuser/someplugin
```

## `text-to-midi plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ text-to-midi plugins:link PLUGIN

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
  $ text-to-midi plugins:link myplugin
```

## `text-to-midi plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ text-to-midi plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ text-to-midi plugins unlink
  $ text-to-midi plugins remove
```

## `text-to-midi plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ text-to-midi plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ text-to-midi plugins unlink
  $ text-to-midi plugins remove
```

## `text-to-midi plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ text-to-midi plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ text-to-midi plugins unlink
  $ text-to-midi plugins remove
```

## `text-to-midi plugins update`

Update installed plugins.

```
USAGE
  $ text-to-midi plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
