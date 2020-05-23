# cwe_checker_ghidra

## Description

This is a simple wrapper script to run cwe_checker (https://github.com/fkie-cad/cwe_checker) with podman or docker and also produce a JSON output file that can be used in Ghidra with cwe_checker's Ghidra plugin (https://fkie-cad.github.io/cwe_checker/doc/html/cwe_checker/index.html#ToolIntegration).

## Installation

```shell
cd ~/.local/bin/
wget https://raw.githubusercontent.com/martinclauss/cwe_checker_ghidra/master/cwe_checker_ghidra
chmod +x cwe_checker_ghidra
```

Make sure that `~/.local/bin` is in your `$PATH`!

## Usage

### Get the JSON Results
```shell

cwe_checker_ghidra <some binary>
```

Error messages from cwe_checker are saved in `cwe_checker_errors.log`. The JSON result is stored in `<some binary>_cwe_hits.js`

### Use with Ghidra

see https://fkie-cad.github.io/cwe_checker/doc/html/cwe_checker/index.html#ToolIntegration
