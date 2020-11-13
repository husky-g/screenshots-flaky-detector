## Prerequisit

You need to install `imagemagick` used to compute diffs:

```
brew install imagemagick
```

## How to use it

### Command

```
screenshots-flaky-detector [options]
```

### Options

| Option          | Description                                                            | Default          |
|-----------------|------------------------------------------------------------------------|------------------|
| `-c`, `--command`   | The command that generates the screenshot, usually a test run          |                  |
| `-n`, `--number`    | The number of screenshot comparison that will be run                   | 5                |
| `-d`, `--directory` | The directory where screenshots are generated by the specified command |                  |
| `-o`, `--output`    | The output directory of the generated diffs if flakies are found       | value specified for `-d` |
| `-v`, `--verbose`   | Verbose mode outputs the specified command outputs                     | `false`            |
