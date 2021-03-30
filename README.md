# ExamplePkg

## Description
sample description

## Usage

### Fetch the package
`kpt pkg get https://github.com/phanimarupaka/examplepkg.git@v0.1.0 ./`

// This step will also configure `settings.json` of vscode to point to extensions in Kptfile

### Open package in vscode, input function parameter values in values.yaml and render
`kpt fn render examplepkg`

### Apply the package
```
kpt live init examplepkg
kpt live apply examplepkg --reconcile-timeout=2m --output=table
```
Details: https://googlecontainertools.github.io/kpt/reference/live/
