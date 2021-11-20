# Automation
## Regular Expression :

A regular expression is a special sequence of characters that helps you match or find other strings or sets of strings, using a specialized syntax held in a pattern.

The Python module re provides full support for Perl-like regular expressions in Python. The re module raises the exception re.error if an error occurs while compiling or using a regular expression.

### The match Function :

This function attempts to match RE pattern to string with optional flags.

Here is the syntax for this function :

```python
re.match(pattern, string, flags=0)
```

1. *`pattern`* : This is the regular expression to be matched.
2. *`string`* : This is the string, which would be searched to match the pattern at the beginning of string.
3. *`flags`* : You can specify different flags using bitwise OR (|). These are modifiers, which are listed in the table below.

### The search Function :

This function searches for first occurrence of RE pattern within string with optional flags.

Here is the syntax for this function :

```python
re.search(pattern, string, flags=0)
```

### Search and Replace :

One of the most important re methods that use regular expressions is *`sub`*.

Here is the syntax for this function :

```python
re.sub(pattern, repl, string, max=0)
```

This method replaces all occurrences of the RE pattern in string with repl, substituting all occurrences unless max provided. This method returns modified string.

![Regular Expressions](https://data-flair.training/blogs/wp-content/uploads/sites/2/2018/02/Regular-Expressions-in-Python-01.jpg)

## Shutil :

The shutil module helps you automate copying files and directories.

This saves the steps of opening, reading, writing and closing files when there is no actual processing.

It is a utility module which can be used to accomplish tasks, such as: copying, moving, or removing directory trees.


copy() method in Python is used to copy the content of source file to destination file or directory.

It also preserves the file's permission mode but other metadata of the file like the file's creation and modification times is not preserved.

![Shutil](https://data-flair.training/blogs/wp-content/uploads/sites/2/2018/06/How-Python-Copy-a-File-01.jpg)