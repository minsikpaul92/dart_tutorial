# Dartpedia

A Wikipedia CLI app built by following the [Dart Tutorial](https://dart.dev/learn/tutorial) by Google.

Searches Wikipedia and reads articles directly from the terminal.

## Project Structure

This is a Dart workspace made up of three packages:

- **`wikipedia/`** — Wikipedia API client (search, article, summary)
- **`command_runner/`** — Custom CLI command runner framework
- **`cli/`** — The actual CLI app that wires everything together

## Usage

```sh
cd cli
```

### Search

```sh
dart run bin/cli.dart search <term>
```

```sh
dart run bin/cli.dart search dart
```

Add `--im-feeling-lucky` to get a summary of the top result:

```sh
dart run bin/cli.dart search dart --im-feeling-lucky
```

### Read an article

```sh
dart run bin/cli.dart article <title>
```

```sh
dart run bin/cli.dart article "Dart_(programming_language)"
```

### Help

```sh
dart run bin/cli.dart help
```

## Logging

Errors are automatically logged to `cli/logs/` as text files (e.g. `2026_5_5_errors.txt`).

## Requirements

- Dart SDK `^3.11.5`

## Running tests

From each package directory:

```sh
cd wikipedia
dart test
```

## Tutorial

https://dart.dev/learn/tutorial
