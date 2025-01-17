Busybox for Windows Scripts
===========================

Some utility scripts for Busybox for Windows.

## Help

dialog-w

    Usage: dialog-w [DIALOG-CMDS...]
    
    Wrapper around dialog(1) for windows. This script downloads dialog
    if needed and executes it. When sourced it provides:
    
      dialog_clear   : Clear screen.
      dialog_SEL ... : Execute dialog, save result in SEL.
      dialog ...     : Execute dialog.

wcompat

    Usage: wcompat ...
    
    ... chkadmin              : Print error when not an administrator.
    ... fetch OFILE URL       : Download a file using wget(1).
    ... fetch-INS   URL       : Download a file ans set $INS to it's pathname.
    ... msiexec-i MSI ARGS... : Install MSI file.
    ... start FILE            : Open file with start.
    ... explorer FILE         : Open file with explorer.
    ... wrapper NAME < CODE   : Create script in WindowsApps/System32 directory.
    ... g-exec CMD            : Execute with a GUI using schtasks when in SSH shell.
    
    Some compativility functions to be used with the Windows Busybox shell.

wsudo

    Usage: wsudo [-u USER] COMMAND
    
    Execute command elevated using the local SSHD server to do the
    elevation.

wterm

    Usage: wterm [COMMAND]

## Collaborating

For making bug reports, feature requests, support or consulting visit
one of the following links:

1. [gemini://harkadev.com/oss/](gemini://harkadev.com/oss/)
2. [https://harkadev.com/oss/](https://harkadev.com/oss/)
