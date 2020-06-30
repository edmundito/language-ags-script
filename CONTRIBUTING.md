## Requirements

- Atom 1.32+
- Node 10.x (**Current version supported by Atom**)

## WORK IN PROGRESS Install Instructions

**This project is still in development** and depends on [tree-sitter-ags-script](https://github.com/edmundito/tree-sitter-ags-script) which 
has not been published to npm yet.

In order to use this module in Atom, you have to
clone `tree-sitter-ags-script` and this repo, link them together, and then install it into Atom as follows:

```sh
git clone git@github.com:edmundito/tree-sitter-ags-script.git
git clone git@github.com:edmundito/language-ags-script.git

cd tree-sitter-ags-script
npm install
npm link

cd ../language-ags-script
npm link tree-sitter-ags-script

apm link .
```

Then you can open Atom.

If you would like to modify the code you can open this project in Atom and
then press `Control(Command on Mac)+P` and type `Window: Reload`.

## Publishing

See: https://flight-manual.atom.io/hacking-atom/sections/publishing/
