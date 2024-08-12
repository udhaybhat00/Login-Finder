# Website Admin Finder Tool 🕵️‍♂️🔍

A simple tool for discovering potential admin login pages and sensitive directories on a target website.

## Features ✨

- **Robots.txt Check:** Determines if the target website has a `robots.txt` file which may contain sensitive information. 🤔
- **Customizable Scanning:** Supports custom file types and path prefixes. 🛠️
- **Multithreading Support:** Offers a fast scanning option using multiple threads. ⚡
- **Custom Wordlists:** Allows you to use a custom wordlist file for scanning. 📜

## Requirements 📝

- **Python:** This tool is written in Python and requires Python 3.x to run. However, the provided executable does not need Python installed on the target machine. 🐍
- **Libraries:** The executable includes all necessary libraries, so you don’t need to install any additional Python packages. 📦

## Installation 💻

### On Linux

1. **Download the Script:** Obtain the Python script version of the tool from the release section or clone the repository.
   ```bash
   https://github.com/udhaybhat00/Login-Finder.git
   unzip LoginFinder
   cd LoginFinder
   ```

2. **Install Python (if not installed):**
   ```bash
   sudo apt update
   sudo apt install python3 python3-pip
   ```

3. **Install Dependencies:**
   ```bash
   pip3 install requests
   ```

4. **Make the Script Executable (Optional):**
   ```bash
   chmod +x LoginFinder.py
   ```

### On Windows

1. **Download the Executable:** Obtain the Windows executable version of the tool from the release section. 📥

2. **Run the Executable:** 
   - Simply double-click the executable file to launch the tool. 🖱️

## Usage 🚀

### On Linux

1. **Launch the Tool:** Open a terminal and navigate to the directory where the script is located. 🏁

2. **Enter the Target URL:** 
   - Input the URL of the website you wish to scan (e.g., `https://example.com`). The tool will automatically adjust the URL format if needed. 🌐

3. **Custom Path Prefix (Optional):**
   - If your target website uses a custom path prefix, enter it here. Leave blank if not needed. 🗂️

4. **Robots.txt Check:** 
   - The tool will check for a `robots.txt` file and display its content if found. This file may contain useful information about the website's structure. 📄

5. **Select Scan Type:**
   - Choose the type of files to scan for: `html`, `asp`, `php`, or `all`. The tool will use this information to filter paths. 🔎

6. **Custom Wordlist (Optional):**
   - Specify the path to a custom wordlist file. If left blank, the default `paths.txt` will be used. 📂

7. **Choose Scanning Speed:**
   - Decide whether to use fast (multithreaded) scanning or a slower single-threaded process. 🚀⚙️

8. **Review Results:** 
   - The tool will display results indicating potential admin panels, directories, and other findings based on the scan. 📊

**Example Commands:**

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

### On Windows

1. **Launch the Tool:** Open the executable to start the tool. 🏁

2. **Enter the Target URL:** 
   - Input the URL of the website you wish to scan (e.g., `https://example.com`). The tool will automatically adjust the URL format if needed. 🌐

3. **Custom Path Prefix (Optional):**
   - If your target website uses a custom path prefix, enter it here. Leave blank if not needed. 🗂️

4. **Robots.txt Check:** 
   - The tool will check for a `robots.txt` file and display its content if found. This file may contain useful information about the website's structure. 📄

5. **Select Scan Type:**
   - Choose the type of files to scan for: `html`, `asp`, `php`, or `all`. The tool will use this information to filter paths. 🔎

6. **Custom Wordlist (Optional):**
   - Specify the path to a custom wordlist file. If left blank, the default `paths.txt` will be used. 📂

7. **Choose Scanning Speed:**
   - Decide whether to use fast (multithreaded) scanning or a slower single-threaded process. 🚀⚙️

8. **Review Results:** 
   - The tool will display results indicating potential admin panels, directories, and other findings based on the scan. 📊

**Example Commands:**

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

## Troubleshooting ⚠️

- **Robots.txt Not Found:** If the tool cannot find a `robots.txt` file, ensure the URL is correct and that the file is accessible. 🔍
- **Request Failed:** If a request fails, it may be due to network issues or incorrect URLs. Verify the target website is reachable. 🌐

## Contributing 🤝

If you'd like to contribute to the development of this tool, feel free to submit pull requests or open issues on the project's repository. 🛠️

## License 📜

This tool is provided as-is under the [MIT License](LICENSE). 🆓

## Contact 📧

For any questions or feedback, please contact me at [udhaybhat00@gmail.com](mailto:udhaybhat00@gmail.com). 📬
