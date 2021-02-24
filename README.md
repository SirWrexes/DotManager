# DotManager: configs made easy #

### Usage ###

```
dot show [supported | installed | saved]
dot save [all | <app>] [<name>] [<user>] [-f | --force] [--nolink]
dot load [all | <app>] [<name>] [<user>] [-f | --force] [--nolink]
dot rm   [all | <app>] [<name>] [<user>] [-f | --force]

Options:
  -h --help     Show this message and exit.
  -V --version  Show version.
  -f --force    Overwrite existing configurations.
  --nolink      Prefer copying files instead of using symlinks.
                Enabled by default for now... Because links are
                not yet implemented LUL.

Commands:
  show:
    supported  Apps that DotManager has a dotinfo for.
    installed  Supported apps that is intalled on your machine.
    saved      Configurations that you have saved.
    
  save, load & rm:
    [all| <app>]  Choose which app to save the configuration of.
                   - If `all`, save every installed apps' configurations.
                   - If the name of a supported app, save its configurations.
                   - If left empty, go through the list of available
                     choices interactively.

    [<name>]      Name of the configuration.
                  Default: "default"

    [<user>]      "Owner" of the configuration.
                  Default: Your username
```

### Upcoming features ###

- Use symlinks to load a config
- Menus for mass operations like `dot save all` etc
- Verbosity
- Easily backup/restore everything with a tar archive
- Saving said archive to OAuth storages like Drive, DropBox...
- Repository support (Gitlab & Github)
- Configuration file
- More as development progresses 😏

### Installation ###

For now, this package is available through test.PyPi.  
Use `pip install -U -i 'https://test.pypi.org/simple' DotManager`  
Lots of things are missing but don't worry, it's coming.  
I have great plans !
