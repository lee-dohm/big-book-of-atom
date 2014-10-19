# The Atom Philosophy

The philosophy behind Atom boils down to two key tenets. Atom is built on Web technologies and it is designed to be very modular.

## Built on Web Technologies

Atom is built on top of two key technologies, Chromium and Node.js. Chromium is the open-source framework upon which Google's Chrome browser is built, it provides the most basic parts of the UI system. Node.js is an engine that provides a stand-alone system for writing JavaScript applications, this gives Atom a framework for writing code that interfaces with the underlying operating system and also forms the basis of Atom's package system. Because of these underpinnings, the code of Atom is written almost completely in CoffeeScript or JavaScript and the UI is a standard combination of HTML and CSS/LESS.

What this allows is twofold:

1. For people who are already familiar with these technologies, their knowledge is immediately portable to Atom. The only thing that needs to be learned is the API and the conventions of the Atom framework.
1. For people who haven't been doing Web work, there is a *ton* of reference material and tutorials on the Web that are directly applicable. This means that they can get up to speed *fast*.

## Modular

Speaking of Atom's package system, Atom is built in such a way that the majority of Atom's functionality, beyond the most very basic text editing capabilities, is provided as a "package". Packages are self-contained bits of code and configuration that can be installed, uninstalled and updated using apm, the Atom Package Manager, or through the Settings View. There is also a [package registry][packages] where one can discover new packages or find out more information about the packages that one already has installed. As of this writing, there are more than 70 packages built-in to Atom's default installation. Each package can provide one or more of the following:

* Code
* Commands
* Key Bindings
* Menus
* Stylesheets
* Snippets

[packages]: https://atom.io/packages
