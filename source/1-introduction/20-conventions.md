# Conventions

This book uses typographic conventions for code, keyboard shortcuts and command-line sections. Keyboard shortcuts (also called "accelerators" on some platforms) are called "key bindings" by Atom. So that is how this book will refer to them as well.

## Code

This book will cover a number of topics that will require writing some amount of code. When code is presented inline, it will be rendered in a monospace font, like this: `foo = 5`. When a block of code is presented, it will be set apart in a block and colorized like this:

```coffeescript
'global':
  'editor':
    'fontFamily': 'SourceCodePro-Light'
    'preferredLineLength': 100
    'invisibles':
      'cr': '↩'
      'tab': '⇥'
      'eol': ' '
    'normalizeIndentOnPaste': false
    'showInvisibles': true
    'scrollPastEnd': true
```

## Key Bindings

Key bindings will be rendered in a boxed monospaced format like this <kbd>Ctrl+X</kbd>. Because Atom is a cross-platform editor and because different platforms use different key bindings, and also because key bindings are so easy to change, we will *not* be referring to the key bindings of Atom commands in this text. In the section on key bindings, we will talk about how to determine what the key binding for a command is and how to set one or change one. But because it is occasionally helpful to refer to key bindings in the generic, there are some conventions we will follow:

* Letter keys will always be referred to in their capital form: <kbd>A</kbd>, <kbd>Z</kbd>
* Modifier keys will have an initial capital and use their common abbreviation: <kbd>Ctrl</kbd>, <kbd>Alt</kbd>
* Special keys such as Tab will be written in all caps: <kbd>TAB</kbd>
* When keys are intended to be held down together such as the Control key and the X key at the same time, they will be joined by a plus sign "+": <kbd>Ctrl+X</kbd>
* When keys are to be pressed separately, they will be separated by a space: <kbd>G I</kbd>

## Command-Line Sections

Command-line sections are blocks that represent a set of actions that are to be taken at the command-line of your respective operating system. This book uses the Unix convention of representing a command-line prompt with a dollar sign (`$`). All command-line examples will be written using Bash-compatible commands for simplicity. Command-line sections will be set apart in a block and colorized similarly to code blocks:

```bash
$ cp foo bar
```
