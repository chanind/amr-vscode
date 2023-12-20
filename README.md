# AMR VSCode

VSCode syntax highlighting for Abstract Meaning Representation (AMR)

## About

[Abstract meaning representation](https://amr.isi.edu/index.html) is a representation of an English sentence as a directed graph, and is typically represented in text like below:

```
(w / want-01
  :ARG0 (b / boy)
  :ARG1 (g / go-01
          :ARG0 b))
```

This VSCode extension provides syntax highlighting for AMR text, and will be automatically enabled for text files with a `.amr` or `.text.amr` file extension.

## Development

This project uses [vscode-tmgrammar-test](https://github.com/PanAeon/vscode-tmgrammar-test) to run snapshot tests of grammar parsing. You can run these tests with `npm run test`. If you make changes to the grammar, you'll need to update these snapshots with `npm run test -- --updateSnapshot`.

To load the grammar in a live vscode editor for debugging, press `F5` with the project open in VSCode and a new window with the extension loaded will open up.

## Contributing

Contributions are welcome! Open a pull request with your changes, and ensure tests are passing.

**Enjoy!**
