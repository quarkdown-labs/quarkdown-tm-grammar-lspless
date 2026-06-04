# Quarkdown LSP-less Grammar

This is an extension of the base Quarkdown TM Grammar used in the VS Code extension. That grammar provides markup highlighting, and is built for integrating with the Quarkdown LSP, which provides semantic tokens of function calls.

This grammar adds *heuristic* highlighting for function calls for environments that don't expect an LSP, such as github/linguist. Since it's a heuristic matching of a context-dependent feature, there may be false positives.

### Building

To generate the main grammar:

```console
npm install
npm run build
```

### Testing

To run the grammar tests:

```console
npm run test
```

The test cases are stored as markdown files under `test/colorize-fixtures`. Grammar test results are stored under `test/colorize-results`, which are automatically generated from the fixtures.

To test the grammar in VS Code, select the `Launch Extension` configuration in the VS Code debugger and run.
