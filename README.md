my-udm-dl
=================

A CLI based tool to download udemy videos for personal use using valid credentials


[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/my-udm-dl.svg)](https://npmjs.org/package/my-udm-dl)
[![Downloads/week](https://img.shields.io/npm/dw/my-udm-dl.svg)](https://npmjs.org/package/my-udm-dl)


<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g my-udm-dl
$ my-udm-dl COMMAND
running command...
$ my-udm-dl (--version)
my-udm-dl/0.0.0 darwin-arm64 node-v20.17.0
$ my-udm-dl --help [COMMAND]
USAGE
  $ my-udm-dl COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`my-udm-dl hello PERSON`](#my-udm-dl-hello-person)
* [`my-udm-dl hello world`](#my-udm-dl-hello-world)
* [`my-udm-dl help [COMMAND]`](#my-udm-dl-help-command)
* [`my-udm-dl plugins`](#my-udm-dl-plugins)
* [`my-udm-dl plugins add PLUGIN`](#my-udm-dl-plugins-add-plugin)
* [`my-udm-dl plugins:inspect PLUGIN...`](#my-udm-dl-pluginsinspect-plugin)
* [`my-udm-dl plugins install PLUGIN`](#my-udm-dl-plugins-install-plugin)
* [`my-udm-dl plugins link PATH`](#my-udm-dl-plugins-link-path)
* [`my-udm-dl plugins remove [PLUGIN]`](#my-udm-dl-plugins-remove-plugin)
* [`my-udm-dl plugins reset`](#my-udm-dl-plugins-reset)
* [`my-udm-dl plugins uninstall [PLUGIN]`](#my-udm-dl-plugins-uninstall-plugin)
* [`my-udm-dl plugins unlink [PLUGIN]`](#my-udm-dl-plugins-unlink-plugin)
* [`my-udm-dl plugins update`](#my-udm-dl-plugins-update)

## `my-udm-dl hello PERSON`

Say hello

```
USAGE
  $ my-udm-dl hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ my-udm-dl hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/saiayyappa/my-udm-dl/blob/v0.0.0/src/commands/hello/index.ts)_

## `my-udm-dl hello world`

Say hello world

```
USAGE
  $ my-udm-dl hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ my-udm-dl hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/saiayyappa/my-udm-dl/blob/v0.0.0/src/commands/hello/world.ts)_

## `my-udm-dl help [COMMAND]`

Display help for my-udm-dl.

```
USAGE
  $ my-udm-dl help [COMMAND...] [-n]

ARGUMENTS
  COMMAND...  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for my-udm-dl.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v6.2.11/src/commands/help.ts)_

## `my-udm-dl plugins`

List installed plugins.

```
USAGE
  $ my-udm-dl plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ my-udm-dl plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/index.ts)_

## `my-udm-dl plugins add PLUGIN`

Installs a plugin into my-udm-dl.

```
USAGE
  $ my-udm-dl plugins add PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into my-udm-dl.

  Uses npm to install plugins.

  Installation of a user-installed plugin will override a core plugin.

  Use the MY_UDM_DL_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the MY_UDM_DL_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ my-udm-dl plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ my-udm-dl plugins add myplugin

  Install a plugin from a github url.

    $ my-udm-dl plugins add https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ my-udm-dl plugins add someuser/someplugin
```

## `my-udm-dl plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ my-udm-dl plugins inspect PLUGIN...

ARGUMENTS
  PLUGIN...  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ my-udm-dl plugins inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/inspect.ts)_

## `my-udm-dl plugins install PLUGIN`

Installs a plugin into my-udm-dl.

```
USAGE
  $ my-udm-dl plugins install PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into my-udm-dl.

  Uses npm to install plugins.

  Installation of a user-installed plugin will override a core plugin.

  Use the MY_UDM_DL_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the MY_UDM_DL_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ my-udm-dl plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ my-udm-dl plugins install myplugin

  Install a plugin from a github url.

    $ my-udm-dl plugins install https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ my-udm-dl plugins install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/install.ts)_

## `my-udm-dl plugins link PATH`

Links a plugin into the CLI for development.

```
USAGE
  $ my-udm-dl plugins link PATH [-h] [--install] [-v]

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ my-udm-dl plugins link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/link.ts)_

## `my-udm-dl plugins remove [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ my-udm-dl plugins remove [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-udm-dl plugins unlink
  $ my-udm-dl plugins remove

EXAMPLES
  $ my-udm-dl plugins remove myplugin
```

## `my-udm-dl plugins reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ my-udm-dl plugins reset [--hard] [--reinstall]

FLAGS
  --hard       Delete node_modules and package manager related files in addition to uninstalling plugins.
  --reinstall  Reinstall all plugins after uninstalling.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/reset.ts)_

## `my-udm-dl plugins uninstall [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ my-udm-dl plugins uninstall [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-udm-dl plugins unlink
  $ my-udm-dl plugins remove

EXAMPLES
  $ my-udm-dl plugins uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/uninstall.ts)_

## `my-udm-dl plugins unlink [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ my-udm-dl plugins unlink [PLUGIN...] [-h] [-v]

ARGUMENTS
  PLUGIN...  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-udm-dl plugins unlink
  $ my-udm-dl plugins remove

EXAMPLES
  $ my-udm-dl plugins unlink myplugin
```

## `my-udm-dl plugins update`

Update installed plugins.

```
USAGE
  $ my-udm-dl plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.7/src/commands/plugins/update.ts)_
<!-- commandsstop -->
