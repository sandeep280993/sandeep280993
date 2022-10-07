# Command Parameters Description

Command Parameter Description is another important section that technical writers author when developing CLI documentation. Technical writers must document the Command Parameter Description to inform the user about the permitted operations and values of the CLI Commands.

Command Parameter Description provides information about the CLI command’s sub-operations, arguments and identifier values.

### 1. Definition List Format

The following example shows the Description formats for the configure command syntax.

Command Syntax:

```
Device@NE# configure shelf <shelf-number> [ ip-address <ip-address> |  priority-value < priority-value > ]
```

The following example shows the Definition List table format:

|a|s|
|-----------|----------|
| \<ip-address\> |An IP address to route data to the NE|
| \<priority-value\> |Preference value of the shelf|

### 2. Table Format

The following examples show the table formats:

The most commonly used formats for the command tables are two-column and three-column tables.

|PARAMETER|DESCRIPTION|
|---------|-----------|
|\<ip-address\>|An IP address to route data to the NE|
|\<priority-value\>|Preference value of the shelf|

#### Two-Column Table

|PARAMETER|VALUE|DESCRIPTION|
|----------|-----|----------|
|\<ip-address\>| \<IPv4 \| IPv6\>| An IP address to route data to the NE|
|\<priority-value\>| \<high \| low\>| Preference value of the shelf|

#### Three-Column Table

### 3. Descriptive Format

The following example shows command parameters in descriptive format:

Command: `remove`

Command description: The `remove` command deletes the configuration values of the NE.

Command mode: `Device@NE(Basic)$`

Command syntax: `remove NE [priority-order <high | low> | config-file <filename>]`

Command parameters:

`<priority-order>` — `< high | low >` — Preference value of the shelf

`<config-file>` — `< filename >` — Filename of the configuration file

