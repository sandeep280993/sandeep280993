# Command Messages

Command Messages are one of the important entities in CLI documentation. These messages help a user to validate the configuration changes the user made in CLI. Whenever a command is executed, the CLI validates the command’s structure, syntax, input values and more. After each validation, the CLI returns a message to inform the user about the success of the input command.

I have provided brief description of types of command messages, based on command structure validation, a technical writer comes across when documenting CLI commands.

### Informational Messages

Informational message provides the user the status of the executed configuration and command description. For configuration status, CLI automatically returns a status message. For help information, engineers develop a cmdhelp[^1] command, which provides the functional information of a command to the user. I have used cmdhelp for reference, but engineers in different organizations use different terms to create the help command.
[^1]: The cmdhelp command used here is a dummy command.

The following examples show how Information Messages appear in CLI.

``` code
Configuration update is complete…
Device@NE$
```
##### Example 1: Updating System Configuration

```
Device@NE$ remove filename sample.txt
Done.
Device@NE$
```
##### Example 2: Deleting File

Informational messages are **generally not documented** by technical writers in the reference guides or user manuals as separate sections. But technical writers can use the informational messages to author descriptions for CLI commands.

### Warning Messages

Warning messages warn against the user-initiated configuration activities that can lead to irreversible changes to the system or NE. These messages present the user an opportunity to continue with the action or abort it.

The following example shows how Warning Message appears in the CLI.

```
The changes made are irreversible. Are you sure you want to continue? (y/n)
```
##### Configuration Change Warning Message

Warning messages are **generally not documented by technical writers** in the reference guides or user manuals as separate sections.

### Error Messages

Error messages inform the user about a wrong command input or invalid configuration. These messages are important in CLI documentation, which inform the user about the occurrence of error.

CLI terminal displays error messages in the following scenarios:

- Incomplete command structure
- Wrong configuration change
- Invalid variable input
- Conflicting configuration by multiple users

The following examples show how Error Messages appear in the CLI.

```
Incomplete command structure…
Device@NE$
```

###### Example 1: Command Syntax Error

```
Cannot confirm configuration as parent hierarchy is not valid.
Device@NE$
```

##### Example 2: Wrong Configuration Execution

Unlike UX writing, technical writers cannot develop error messages in CLI. Engineers decide on the CLI error messages as how the project demands. Technical writers cannot provide a human-touch to CLI error messages, but the writers can document CLI error messages in a user-friendly format. Writers can follow the table format to document CLI error messages.

#### Error Message Table

|Error Message |Description |Correction |
|--------------|------------|-----------|
|Incomplete command structure|Command structure or syntax entered by user is not complete|Enter the complete command structure|
|Interface invalid|Interface configured by the user is invalid	|Check for valid interfaces. Refer interface table on how to configure interfaces.|

The table format or the header description in the example is **not the only correct format** to document CLI error messages. Table format is suited for compact documentation of error messages. The writers can author each error message **as an individual section** or use the **Definition List table** to document the messages. However, technical writers are **free to use any format** that helps the user to understand the error.

Error messages are the only messages **documented by technical writers** in the reference guides and user manuals.
