# Command Titles

For technical writers who are confused about CLI command titles, the following basic examples can be useful.

### 1. Command Syntax/Syntax

The Command Syntax title can be used to explain the structure of the command to the user.

#### For Example:
The following command is the IP Configuration command.

Command Syntax:

```
configure ip-type <ipv4 | ipv6> ip-address <ip-address> netmask <netmask-address>
```

The example allows the user to assign a value as per his/her choices.

This command title is used in CLI Reference Guides and sometimes in User Manuals for CLI procedures.

### 2. Command

The Command title can be used for direct commands that cannot be changed by the user and the command shall be used as described in the guide.

#### For Example:

Use the following command to delete the configuration file.

Command:

```
remove configuration file
```

The example restricts the user to make modifications to the command in the CLI terminal.

This command title is used in User Manuals for CLI procedures.

### 3. Command Example

The Command Example title can be used for sample commands in a procedure that describes a task to the user through CLI commands.

#### For Example

Step: Upgrade new configuration software to the remote NE from local directory.

#### Command Example:

```
upgrade CF-1584.DBS from admin@xxx.xxx.xxx.x/local/directory to xxx.xxx.xxx.x/remote/NE/file/directory
```

This command title is used in CLI Reference Guides and in User Manuals for CLI procedures.

### 4. Response

The Response title can be used for CLI messages that prompt the user to take action or inform the user about the completion of tasks.

#### For Example

Step 1: Enter yes to continue.

#### Response:

```
Do you want to continue? (yes/no)
```

Result: The task completes with a following message

#### Response:
```
Operation Successful...
```
This command title is used in User Manuals for CLI procedures.

### 5. Output Example/Output

The Output Example title can be used for sample outputs that inform the audience on how to verify their operations or the response of the operation from the configured sample commands.

#### For Example

Step: Verify the configured IP Address with the following command:

#### Command:
```
display ip
```
#### Output Example:

```
ip 192.154.55.2
```

This command title is used in CLI Reference Guides and in User Manuals for CLI procedures.




