# Changing UI and Syntax Themes

There are two types of theme packages in Atom: UI and Syntax themes. The Syntax theme specifically is for elements that show up in text editor views. It doesn't just determine what colors syntax highlighting uses, though that is its main purpose, but also:

* Gutter elements
    * Line numbers
    * Git diff highlights
    * Fold icons
* Wrap guide
* Find and replace highlight
* Cursor
* etc

The UI theme handles the styling of everything else.

## Changing via Settings View

You can easily change your selected UI and Syntax themes through the Settings View:

1. Open the Settings View
1. Click the Themes tab
1. Select Syntax or UI theme in their respective drop down lists

## Changing via Configuration File

You can change your selected themes via direct editing of the `config.cson`, but it isn't recommended. If you accidentally change to a theme that isn't installed or make a typo, Atom could become unusable.
