# Command Modes

Command Mode is one of the important features to author in CLI documentation. In CLI documentation, technical writers must document the command modes to inform the user on how to manage the product efficiently.
  
For Technical Writers who want to get familiar with CLI documentation, understanding how to document CLI Command Modes can be helpful. I have provided information on how command modes are documented.

Command modes are represented by the Prompts that appear in a CLI window. These Command Prompts reflect the position of the user within the command hierarchy. Command Prompts are designed in different formats. The majority format engineers develop command prompts are the following formats:

`Device@NE$ | Device@NE#` – Command prompt symbols change for different users

`Device@NE(Basic)$ | Device@NE(Privilege)$` – Command prompt descriptions changes for different users

Documenting CLI command modes is up to the technical writers’ discretion. Command Modes can be explained using a table in a separate section. Command Modes can also be added in the sections for commands that are operable within the mode.

The following example shows how to describe command modes in a table:

### Example 1: Command Modes Table

|COMMAND MODE|ENTRY METHOD|PROMPT|EXIT METHOD|
|------------|------------|------|-----------|
|Basic level of operation|Basic|Device@NE$|Enter `end` to exit|
|Advanced level of operation|Privilege|Device@NE#|Enter `end` to exit|

### Example 2: Command Modes in Command Description

Command: `remove`

Command description: The remove command deletes the configuration values of the NE.

Command mode: `Device@NE(Basic)$`

Command syntax: `remove NE [priority-order <high | low> | config-file <filename>]`

The above examples are the commonly used styles for documenting Command Modes. Table format can be used when many command modes exist for a product. Adding Command Mode in command description informs the user in which mode the command should be used. Technical writers can document the Command modes in any format that helps the user to understand the modes.

There is no one correct way to document CLI Command Modes. Technical writers can document the Command Modes in any style that helps the user to understand the modes.
