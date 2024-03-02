# GhostBuster

GhostBuster is a Python script for recursively scanning directories on a web server to find existing directories and determine their accessibility.
<br>
## Features

- Multithreaded scanning for faster directory enumeration
- Support for various HTTP methods (GET, POST, HEAD, PUT, DELETE)
- Automatic detection of open ports (default: 80)
- Progress display showing scanned directories
- Display of found directories in real-time

## Usage

1. **Clone the Repository:**

    ```bash
    git clone https://github.com/your-username/ghostbuster.git
    ```

2. **Navigate to the Project Directory:**

    ```bash
    cd ghostbuster
    ```

3. **Run the Script:**

    ```bash
    python ghostbuster.py <url> [-w WORDLIST]
    ```

    Replace `<url>` with the target URL, `<wordlist>` with the path to your wordlist file.

4. **Example:**

    ```bash
    python ghostbuster.py http://example.com
    ```

## Requirements

- Python 3.x
- requests library (install via `pip install requests`)

## Wordlist

The default wordlist (`directory-list-2.3-medium.txt`) provided by [SecLists](https://github.com/danielmiessler/SecLists) is used. You can also use your custom wordlist by specifying the path using the `-w` option.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
