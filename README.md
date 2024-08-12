# Login Finder for Linux and Windows v1.0

A script to find admin login pages and EAR vulnerabilities.

#### Features
- [x] Multi-threading on demand
- [x] Big path list (482 paths)
- [x] Support custom path list (wordlist)
- [x] Supports PHP, ASP, and HTML extensions
- [x] Checks for potential EAR vulnerabilities
- [x] Checks for `robots.txt`
- [x] Support for custom paths

### Usages

#### On Linux

- **Check all paths with PHP extension:**
  ```bash
  python LoginFinder.py -u example.com --type php
  ```

- **Check all paths with PHP extension using threads:**
  ```bash
  python LoginFinder.py -u example.com --type php --fast
  ```

- **Check all paths without using threads:**
  ```bash
  python LoginFinder.py -u example.com
  ```

- **Add a custom path. For example, if you want all paths to start with `/data` (e.g., `example.com/data/...`):**
  ```bash
  python LoginFinder.py -u example.com --path /data
  ```

#### On Windows

- **Check all paths with PHP extension:**
  ```cmd
  python LoginFinder.py -u example.com --type php
  ```

- **Check all paths with PHP extension using threads:**
  ```cmd
  python LoginFinder.py -u example.com --type php --fast
  ```

- **Check all paths without using threads:**
  ```cmd
  python LoginFinder.py -u example.com
  ```

- **Add a custom path. For example, if you want all paths to start with `/data` (e.g., `example.com/data/...`):**
  ```cmd
  python LoginFinder.py -u example.com --path /data
  ```

### Installation

1. **Download and Extract:**
   - **Linux:** Download the script and make sure you have Python 3 installed.
   - **Windows:** Download the executable or script and ensure Python 3 is installed.

2. **Install Dependencies (if using the script):**
   ```bash
   pip install requests
   ```

3. **Run the Script:**
   - Execute the appropriate command based on your platform from the examples above.

### Additional Notes

- Ensure that Python 3 is installed and added to your system's PATH.
- For the executable version, simply run the `.exe` file without needing Python.

## Contributing

Feel free to submit pull requests or open issues if you encounter any problems or have suggestions for improvements.

## License

This tool is provided as-is under the [MIT License](LICENSE).

## Contact

For any questions or feedback, please contact me at [udhaybhat00@gmail.com](mailto:udhaybhat00@gmail.com).
