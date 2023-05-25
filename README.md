# Symbol Prefix Validator for Python Libraries

# Symbol Check

Symbol Check is a Python script that checks exported symbols of libraries for any "smelly" symbols that do not adhere to specific prefix conventions. It utilizes the `nm` command-line tool to extract symbol information from dynamic libraries and performs checks to ensure that symbols are properly prefixed.

## Requirements

- Python 3.x
- `nm` command-line tool (typically available on Unix-like systems)

## Usage

1. Clone the repository or download the `symbol_check.py` file.

2. Open a terminal or command prompt and navigate to the directory containing `symbol_check.py`.

3. Run the script using the following command:

   ```shell
   python symbol_check.py

The script will analyze the exported symbols of libraries and provide the following information:

The number of local symbols ignored
Any smelly symbols found
The total number of smelly symbols found
If no smelly symbols are found, the script will display a success message.

Review the output to identify any smelly symbols that require attention.

# Configuration

The script has the following configuration options:

ALLOWED_PREFIXES: A tuple of allowed symbol prefixes. By default, it includes 'Py' and '_Py'. Additional prefixes can be added as needed.

IGNORED_EXTENSION: A string representing an extension that should be ignored when checking extension modules.

IGNORED_SYMBOLS: A set of symbols that should be ignored when checking symbols.

# Contributing

Contributions to Symbol Check are welcome! If you find any issues or have suggestions for improvements, please open an issue or submit a pull request on the GitHub repository.


