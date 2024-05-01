# bash-command-printer
A minimal bash script to print each command being run in a bash script

## Getting started

Getting started with the command printer is easy! Just source the
`command-printer` file and run the `activate_command_printer` function. That's
it!

```bash
#!/usr/bin/env bash

# To activate the command printer
. command-printer
activate_command_printer

# Your script here
echo "Hello world"
```

You can also choose to activate the command printer later in the script if you
don't care about printing e.g. setup commands:

```bash
#!/usr/bin/env bash

# To activate the command printer
. command-printer

# Your setup code

activate_command_printer

# Your script here
echo "Hello world"
```

## Examples
### Hello world
[examples/01_hello_world/hello_world](examples/01_hello_world/hello_world)
![](examples/01_hello_world/hello_world.gif)

### Variable expansion
[examples/02_variable_expansion/variable_expansion](examples/02_variable_expansion/variable_expansion)
![](examples/02_variable_expansion/variable_expansion.gif)

[examples/03_command_substitution/command_substitution](examples/03_command_substitution/command_substitution)
![](examples/03_command_substitution/command_substitution.gif)

### Multiple commands on the same line
[examples/04_multiple_commands/multiple_commands](examples/04_multiple_commands/multiple_commands)
![](examples/04_multiple_commands/multiple_commands.gif)

[examples/04_multiple_commands/multiple_commands_split](examples/04_multiple_commands/multiple_commands_split)
![](examples/04_multiple_commands/multiple_commands_split.gif)

### `if` statements
[examples/05_if_statements/if_statements](examples/05_if_statements/if_statements)
![](examples/05_if_statements/if_statements.gif)

### Loops
[examples/06_loops/while_loop](examples/06_loops/while_loop)
![](examples/06_loops/while_loop.gif)

[examples/06_loops/range_loop](examples/06_loops/range_loop)
![](examples/06_loops/range_loop.gif)

### Show for how long time a command runs
[examples/07_long_running_commands/no_report](examples/07_long_running_commands/no_report)
![](examples/07_long_running_commands/no_report.gif)

[examples/07_long_running_commands/with_report](examples/07_long_running_commands/with_report)
![](examples/07_long_running_commands/with_report.gif)
