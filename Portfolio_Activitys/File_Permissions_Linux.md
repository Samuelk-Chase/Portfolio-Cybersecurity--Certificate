# Linux File Permissions

## Project Description

This project demonstrates how to manipulate file and directory permissions in Linux using command-line tools. It covers checking file and directory details, describing the permissions string, changing file permissions, changing file permissions on a hidden file, and changing directory permissions.

## Check File and Directory Details

To check file and directory details in Linux, you can use the `ls` command with the `-l` option. This provides a detailed listing that includes permissions, ownership, size, and modification time.

```bash
ls -l <file_or_directory>
```

To list all files, including hidden ones, you can use the `-a` option:

```bash
ls -a
```

And for a detailed listing of all files, including hidden ones, you can use both `-l` and `-a` options together:

```bash
ls -la
```

## Describe the Permissions String

The permissions string in Linux consists of ten characters, representing the file type and permissions for the owner, group, and others. The characters are divided into three groups of three:
- The first character represents the file type.
- The next three characters represent permissions for the owner.
- The following three characters represent permissions for the group.
- The last three characters represent permissions for others.

For example, `drwxr-xr-x` indicates a directory (`d`) with read, write, and execute permissions for the owner, and read and execute permissions for both the group and others.

## Change File Permissions

To change file permissions in Linux, you can use the `chmod` command followed by the desired permissions mode and the filename.

```bash
chmod <permissions_mode> <filename>
```

For example, to give read, write, and execute permissions to the owner of a file named `example.txt`, you can use:

```bash
chmod u+rwx example.txt
```

## Change File Permissions on a Hidden File

To change permissions on a hidden file (one whose name starts with a dot), you can specify the filename directly with the `chmod` command.

```bash
chmod <permissions_mode> .<filename>
```

For example, to give read and write permissions to the owner of a hidden file named `.hidden`, you can use:

```bash
chmod u+rw .hidden
```

## Change Directory Permissions

To change directory permissions in Linux, you can also use the `chmod` command, similar to changing file permissions.

```bash
chmod <permissions_mode> <directory_name>
```

For example, to give read, write, and execute permissions to the owner of a directory named `my_directory`, you can use:

```bash
chmod u+rwx my_directory
```

## Summary

This file provides a brief overview of managing file and directory permissions in Linux through command-line tools. Refer to the specific sections for detailed instructions and examples.
